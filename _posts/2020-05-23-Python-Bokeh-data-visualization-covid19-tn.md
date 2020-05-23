---
layout: post
title:  "Python-Bokeh Data Visualization"
date:   2020-05-23 21:00:00 +0530
categories: jekyll update


---

<p>
I am sharing below the python codes for the data visualiztion of the COVID19 outbreak in Tamil Nadu in my previous most. Please note that I'm not a professional programmer and so, the codes could be considered crude by expert coders. I hope my codes don't scare them too much. The programs are meant to just about work and far from being memory-efficient. So, tread with caution! All of the plots have interactive tooltips on hovering. The last plot uses a dropdown selection menu which allows users to select an option among many and the appropriate graph appears. The data along with the codes can also be found here: https://github.com/aksaba/MyCodes/tree/master/Py/DataVisualisation/TNCOVID19
</p>
<p>
Cumulative and Daily cases - bar graphs
</p>
<pre>
<code>

########################################################################
## Two bar graphs arranged one below the other
## Interactive tooltips
########################################################################

from bokeh.plotting import output_file,save,figure,show
from bokeh.layouts import column
from bokeh.models import DatetimeTickFormatter,ranges,Dropdown, SingleIntervalTicker,Label,HoverTool,ColumnDataSource,FactorRange

import csv
import numpy as np
output_file('vbar_cumulative_daily.html')
with open("Book2.csv") as csvfile:  ## Read csv file
    csvdata = list(csv.reader(csvfile))

DATE = [item[0] for item in csvdata]
POS_COUNT = [item[1] for item in csvdata]
DAILY_POS_COUNT = [item[2] for item in csvdata]
data = {'DATE' : DATE,
        'POS_COUNT': POS_COUNT,
        'DAILY_POS_COUNT':DAILY_POS_COUNT}
x = data['DATE']
pos_counts = data['POS_COUNT']
daily_counts = data['DAILY_POS_COUNT']

source = ColumnDataSource(data=dict(x=x, pos_counts=pos_counts,daily_counts=daily_counts))

mytext1_ypos = int(pos_counts[len(pos_counts)-1])-600
mytext1 = Label(x=1, y=mytext1_ypos, text='Day 0 (first detected case): 07 March 2020')

plot1 = figure(x_range=FactorRange(*x),plot_width=700,plot_height=350,title="Number of positive cases (Cumulative)")
plot1.vbar('x', top='pos_counts', width=0.9, source=source)
plot1.title.text_font_size = "15pt"
plot1.xaxis.axis_label = "Day"
plot1.xaxis.axis_label_text_font = "times"
plot1.xaxis.axis_label_text_font_style = "normal"
plot1.xaxis.major_label_text_font_size = "10pt"
plot1.xaxis.major_label_orientation = np.pi/2
plot1.xaxis.axis_label_text_font_size = "15pt"
plot1.xaxis.ticker = SingleIntervalTicker(interval=2)
plot1.yaxis.axis_label = "No. of Cases"
plot1.yaxis.axis_label_text_font = "times"
plot1.yaxis.axis_label_text_font_style = "normal"
plot1.yaxis.major_label_text_font_size = "10pt"
plot1.yaxis.axis_label_text_font_size = "15pt"
plot1.add_tools(HoverTool(tooltips=[("DATE", "@x"), ("No. of cases", "@pos_counts")]))
plot1.add_layout(mytext1)

mytext2_ypos = int(daily_counts[len(daily_counts)-1])+20
mytext2 = Label(x=1, y=mytext2_ypos, text='Day 0 (first detected case): 07 March 2020')

plot2 = figure(x_range=x, plot_width=700,plot_height=350,title="Number of daily positive cases")
plot2.vbar(x='x', top='daily_counts', width=0.9, source=source)
plot2.title.text_font_size = "15pt"
plot2.xaxis.axis_label = "Day"
plot2.xaxis.axis_label_text_font = "times"
plot2.xaxis.axis_label_text_font_style = "normal"
plot2.xaxis.major_label_text_font_size = "10pt"
plot2.xaxis.major_label_orientation = np.pi/2
plot2.xaxis.axis_label_text_font_size = "15pt"
plot2.xaxis.ticker = SingleIntervalTicker(interval=2)
plot2.yaxis.axis_label = "No. of Cases"
plot2.yaxis.axis_label_text_font = "times"
plot2.yaxis.axis_label_text_font_style = "normal"
plot2.yaxis.major_label_text_font_size = "10pt"
plot2.yaxis.axis_label_text_font_size = "15pt"
plot2.add_tools(HoverTool(tooltips=[("DATE", "@x"), ("No. of cases", "@daily_counts")]))
plot2.add_layout(mytext2)

save(column(plot1,plot2))

</code>
</pre>

<p>
Total samples tested with %total positive cases and %total active cases - three line plots in the same graph along with a secondary y-axis
</p>
<code>

########################################################################
## Three line plots in the same graph
## Secondary y-axis for one of the plots
## Interactive tooltips for each plot
########################################################################

from bokeh.plotting import output_file,save,figure,show
from bokeh.models import HoverTool,ColumnDataSource,FactorRange,Range1d,LinearAxis,Label,SingleIntervalTicker
import csv
import numpy as np
output_file('vbar_samples.html')
with open("Book2.csv") as csvfile:
    csvdata = list(csv.reader(csvfile))

DATE = [item[0] for item in csvdata]
SAMPLES = [item[3] for item in csvdata]
PERCENT_POS = [item[4] for item in csvdata]
PERCENT_ACT = [item[5] for item in csvdata]
data = {'DATE' : DATE,
        'SAMPLES': SAMPLES,
        'PERCENT_POS':PERCENT_POS,
        'PERCENT_ACT':PERCENT_ACT}
x = data['DATE']
samples = data['SAMPLES']
percent_pos = data['PERCENT_POS']
percent_act = data['PERCENT_ACT']

mytext1_ypos = float(samples[len(samples)-1])-20  # decrease number
mytext1 = Label(x=1, y=mytext1_ypos, text='Day 0 (first detected case): 07 March 2020')
ymax = float(samples[len(samples)-1])+5

plot1 = figure(x_range=x,y_range=(0,ymax),plot_width=700,plot_height=350,title="Samples processed and percentage of positive samples")
plot1.extra_y_ranges = {"foo": Range1d(start=0, end=15)}
plot1.line(x,samples,line_color="green", line_width = 3.5,alpha = 0.75, legend_label = "Processed samples")
plot1.yaxis.axis_label = "No. of Samples (in thousands)"
plot1.add_tools(HoverTool(tooltips=[("DATE", "@x"), ("Value", "@y")]))
plot1.line(x,percent_pos,y_range_name = "foo",line_color="red",line_width = 3.5,alpha = 0.75, legend_label = "% total positive cases")
plot1.line(x,percent_act,y_range_name = "foo",line_color="blue",line_width = 3.5,alpha = 0.75, legend_label = "% active positive cases")
plot1.add_layout(LinearAxis(y_range_name="foo",axis_label="%"), 'right')
plot1.title.text_font_size = "15pt"
plot1.xaxis.axis_label = "Day"
plot1.xaxis.axis_label_text_font = "times"
plot1.xaxis.axis_label_text_font_style = "normal"
plot1.xaxis.ticker = SingleIntervalTicker(interval=2)
plot1.xaxis.major_label_text_font_size = "10pt"
plot1.xaxis.major_label_orientation = np.pi/2
plot1.xaxis.axis_label_text_font_size = "15pt"
plot1.yaxis.axis_label_text_font = "times"
plot1.yaxis.axis_label_text_font_style = "normal"
plot1.yaxis.major_label_text_font_size = "10pt"
plot1.yaxis.axis_label_text_font_size = "15pt"
plot1.add_layout(mytext1)
legend_ypos = float(samples[len(samples)-1])-215  # Decrease number
plot1.legend.location = (1,legend_ypos)
plot1.ygrid.visible = False

save(plot1)

</code>

<p>
Number of deaths and %mortality- bar plot and line plot in the same graph, secondary y-axis
</p>
<code>

########################################################################
## Bar plot and line plot in one graph
## Secondary y-axis for the line plot
## Interactive tooltips
########################################################################

from bokeh.plotting import output_file,save,figure,show
from bokeh.models import HoverTool,ColumnDataSource,FactorRange,Range1d,LinearAxis,DatetimeTickFormatter,ranges, SingleIntervalTicker, Label
import csv
import numpy as np
output_file('vbar_mortality.html')
with open("Book2.csv") as csvfile:
    csvdata = list(csv.reader(csvfile))

DATE = [item[0] for item in csvdata]
DEATH_COUNT = [item[9] for item in csvdata]
DEATH_PERCENT = [item[10] for item in csvdata]
data = {'DATE' : DATE,
        'DEATH_COUNT': DEATH_COUNT,
        'DEATH_PERCENT':DEATH_PERCENT}
x = data['DATE']
death_counts = data['DEATH_COUNT']
death_percent = data['DEATH_PERCENT']
ymax = int(death_counts[len(death_counts)-1])+5
source = ColumnDataSource(data=dict(x=x, death_counts=death_counts,death_percent=death_percent))

mytext1_ypos = int(death_counts[len(death_counts)-1])-5
mytext1 = Label(x=1, y=mytext1_ypos, text='Day 0 (first detected case): 07 March 2020')

plot1 = figure(x_range=x,y_range=(0,ymax),plot_width=700,plot_height=350,title="Number of deaths (Cumulative) and % mortality rate")
plot1.extra_y_ranges = {"foo": Range1d(start=0, end=5)}
plot1.vbar('x', top='death_counts', width=0.9, source=source)
plot1.yaxis.axis_label = "Count"
plot1.line(x,death_percent,y_range_name = "foo",line_color="red", line_width = 3.5,alpha = 0.75, legend_label = "% mortality rate")
plot1.add_layout(LinearAxis(y_range_name="foo",axis_label="%"), 'right')
plot1.title.text_font_size = "15pt"
plot1.xaxis.axis_label = "Day"
plot1.xaxis.axis_label_text_font = "times"
plot1.xaxis.axis_label_text_font_style = "normal"
plot1.xaxis.major_label_text_font_size = "10pt"
plot1.xaxis.major_label_orientation = np.pi/2
plot1.xaxis.axis_label_text_font_size = "15pt"
plot1.xaxis.ticker = SingleIntervalTicker(interval=2)
plot1.yaxis.axis_label_text_font = "times"
plot1.yaxis.axis_label_text_font_style = "normal"
plot1.yaxis.major_label_text_font_size = "10pt"
plot1.yaxis.axis_label_text_font_size = "15pt"
legend_ypos = float(death_counts[len(death_counts)-1])+150  # Decrease number
plot1.legend.location = (1,legend_ypos)
plot1.add_tools(HoverTool(tooltips=[("DATE", "@x"), ("No. of deaths","@death_counts"),("% mortality", "@death_percent")]))
plot1.add_layout(mytext1)

save(plot1)
</code>

<p>
District wise trends - multiple graphs with selection dropdown menu
</p>
<code>

########################################################################
## Multiple bar plots
## Selection box allows user to select an option among several
## Interactive tooltips
########################################################################


from bokeh.plotting import output_file,save,figure,show
from bokeh.models import HoverTool,ColumnDataSource,FactorRange,DatetimeTickFormatter,ranges,Select
from bokeh.models.callbacks import CustomJS
from bokeh.layouts import row
import csv
import numpy as np
output_file('vbar_districts.html')

with open("districts.csv") as csvfile:
    csvdata = list(csv.reader(csvfile))

DATE = [item[0] for item in csvdata]
i = 0
y = []
while i < 37 :
     y.append([item[i+1] for item in csvdata])
     i=i+1
data = {'DATE' : DATE}
x = data['DATE']
source = ColumnDataSource(data=dict(x=x, y=y[0],y0=y[0],y1=y[1],y2=y[2],y3=y[3],y4=y[4],y5=y[5],y6=y[6],y7=y[7],y8=y[8],y9=y[9],y10=y[10],y11=y[11],y12=y[12],y13=y[13],y14=y[14],y15=y[15],y16=y[16],y17=y[17],y18=y[18],y19=y[19],y20=y[20],y21=y[21],y22=y[22],y23=y[23],y24=y[24],y25=y[25],y26=y[26],y27=y[27],y28=y[28],y29=y[29],y30=y[30],y31=y[31],y32=y[32],y33=y[33],y34=y[34],y35=y[35],y36=y[36]))

plot1 = figure(x_range=x,plot_width=550,plot_height=350,title="Number of active cases in the last 21 days")
plot1.vbar('x', top='y', source=source,width = 0.8)
plot1.title.text_font_size = "12pt"
plot1.xaxis.major_label_text_font_size = "10pt"
plot1.xaxis.major_label_orientation = np.pi/2
plot1.xaxis.axis_label_text_font_size = "15pt"
plot1.yaxis.axis_label = "No. of Cases"
plot1.yaxis.axis_label_text_font = "times"
plot1.yaxis.axis_label_text_font_style = "normal"
plot1.yaxis.major_label_text_font_size = "10pt"
plot1.yaxis.axis_label_text_font_size = "15pt"
plot1.add_tools(HoverTool(tooltips=[("DATE", "@x"), ("No. of cases", "@y")]))

callback = CustomJS(args=dict(source=source),code="""
        var data = source.data;
        var f = cb_obj.value
        if(f=="Ariyalur") {source.data['y'] = source.data['y0'];}
        else if(f=="Ariyalur") {source.data['y'] = source.data['y0'];}
        else if(f=="Chengalpattu") {source.data['y'] = source.data['y1'];}
        else if(f=="Chennai") {source.data['y'] = source.data['y2'];}
        else if(f=="Coimbatore") {source.data['y'] = source.data['y3'];}
        else if(f=="Cuddalore") {source.data['y'] = source.data['y4'];}
        else if(f=="Dharmapuri") {source.data['y'] = source.data['y5'];}
        else if(f=="Dindigul") {source.data['y'] = source.data['y6'];}
        else if(f=="Erode") {source.data['y'] = source.data['y7'];}
        else if(f=="Kallakurichi") {source.data['y'] = source.data['y8'];}
        else if(f=="Kancheepuram") {source.data['y'] = source.data['y9'];}
        else if(f=="Kanyakumari") {source.data['y'] = source.data['y10'];}
        else if(f=="Karur") {source.data['y'] = source.data['y11'];}
        else if(f=="Krishnagiri") {source.data['y'] = source.data['y12'];}
        else if(f=="Madurai") {source.data['y'] = source.data['y13'];}
        else if(f=="Nagapattinam") {source.data['y'] = source.data['y14'];}
        else if(f=="Namakkal") {source.data['y'] = source.data['y15'];}
        else if(f=="Nilgiris") {source.data['y'] = source.data['y16'];}
        else if(f=="Perambalur") {source.data['y'] = source.data['y17'];}
        else if(f=="Pudukottai") {source.data['y'] = source.data['y18'];}
        else if(f=="Ramnad") {source.data['y'] = source.data['y19'];}
        else if(f=="Ranipet") {source.data['y'] = source.data['y20'];}
        else if(f=="Salem") {source.data['y'] = source.data['y21'];}
        else if(f=="Sivagangai") {source.data['y'] = source.data['y22'];}
        else if(f=="Tenkasi") {source.data['y'] = source.data['y23'];}
        else if(f=="Thanjavur") {source.data['y'] = source.data['y24'];}
        else if(f=="Theni") {source.data['y'] = source.data['y25'];}
        else if(f=="Thirupathur") {source.data['y'] = source.data['y26'];}
        else if(f=="Thiruvallur") {source.data['y'] = source.data['y27'];}
        else if(f=="Thiruvannamalai") {source.data['y'] = source.data['y28'];}
        else if(f=="Thiruvarur") {source.data['y'] = source.data['y29'];}
        else if(f=="Thoothukudi") {source.data['y'] = source.data['y30'];}
        else if(f=="Tirunelveli") {source.data['y'] = source.data['y31'];}
        else if(f=="Tiruppur") {source.data['y'] = source.data['y32'];}
        else if(f=="Trichy") {source.data['y'] = source.data['y33'];}
        else if(f=="Vellore") {source.data['y'] = source.data['y34'];}
        else if(f=="Villupuram") {source.data['y'] = source.data['y35'];}
        else if(f=="Virudhunagar") {source.data['y'] = source.data['y36'];}
        source.change.emit();

    """)

select = Select(title="Select District:", width =140, value="Ariyalur", options=["Ariyalur","Chengalpattu","Chennai","Coimbatore","Cuddalore","Dharmapuri","Dindigul","Erode","Kallakurichi","Kancheepuram","Kanyakumari","Karur","Krishnagiri","Madurai","Nagapattinam","Namakkal","Nilgiris","Perambalur","Pudukottai","Ramnad","Ranipet","Salem","Sivagangai","Tenkasi","Thanjavur","Theni","Thirupathur","Thiruvallur","Thiruvannamalai","Thiruvarur","Thoothukudi","Tirunelveli","Tiruppur","Trichy","Vellore","Villupuram","Virudhunagar"])
select.js_on_change('value', callback)
save(row(select,plot1))

</code>