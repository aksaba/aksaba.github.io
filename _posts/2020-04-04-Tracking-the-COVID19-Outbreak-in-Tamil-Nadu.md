---
layout: post
title:  "Tracking the COVID19 outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<p>Graphs updated: 2115 hours 05 May 2020 </p>





<!DOCTYPE html>
<html lang="en">
  
  <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="5de6cd8c-0705-4856-8d04-276ae096741a" data-root-id="1004"></div>
            
          
        
      
      
        <script type="application/json" id="1128">
          {"55415aa0-78e5-4d76-b05c-4b859d55393c":{"roots":{"references":[{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1040"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1046"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1048","type":"UnionRenderers"},{"attributes":{},"id":"1049","type":"Selection"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1042"}]},"id":"1028","type":"Toolbar"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@pos_counts"]]},"id":"1042","type":"HoverTool"},{"attributes":{"interval":2},"id":"1040","type":"SingleIntervalTicker"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"id":"1003","type":"FactorRange"},{"attributes":{"source":{"id":"1001"}},"id":"1039","type":"CDSView"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":3958},"id":"1002","type":"Label"},{"attributes":{"data":{"daily_counts":["1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105","43","76","33","54","72","66","64","52","121","104","161","203","231","266","527","508"],"pos_counts":["1","1","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477","1520","1596","1629","1683","1755","1821","1885","1937","2058","2162","2323","2526","2757","3023","3550","4058"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"selected":{"id":"1049"},"selection_policy":{"id":"1048"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{},"id":"1046","type":"BasicTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1002"}],"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"}],"title":{"id":"1005"},"toolbar":{"id":"1028"},"x_range":{"id":"1003"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1004","subtype":"Figure","type":"Plot"},{"attributes":{"text":"Number of positive cases (Cumulative)","text_font_size":{"value":"15pt"}},"id":"1005","type":"Title"},{"attributes":{},"id":"1047","type":"CategoricalTickFormatter"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1012","type":"LinearScale"},{"attributes":{},"id":"1008","type":"DataRange1d"}],"root_ids":["1004"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1128').textContent;
                  var render_items = [{"docid":"55415aa0-78e5-4d76-b05c-4b859d55393c","root_ids":["1004"],"roots":{"1004":"5de6cd8c-0705-4856-8d04-276ae096741a"}}];
                  root.Bokeh.embed.embed_items(docs_json, render_items);
                
                  }
                  if (root.Bokeh !== undefined) {
                    embed_document(root);
                  } else {
                    var attempts = 0;
                    var timer = setInterval(function(root) {
                      if (root.Bokeh !== undefined) {
                        clearInterval(timer);
                        embed_document(root);
                      } else {
                        attempts++;
                        if (attempts > 100) {
                          clearInterval(timer);
                          console.log("Bokeh: ERROR: Unable to run BokehJS code because BokehJS library is missing");
                        }
                      }
                    }, 10, root)
                  }
                })(window);
              });
            };
            if (document.readyState != "loading") fn();
            else document.addEventListener("DOMContentLoaded", fn);
          })();
        </script>
    
  </body>
  
</html>


<div style="text-align:justify">

<p> 04 April 2020 </p>
<p>
This is day 10 of the lock down which is in effect because of the worldwide COVID19 outbreak. I'm in the last stretch of my doctoral research and I have hit a roadblock. Using my laptop and remote computing, some progress was possible in the last 10 to 15 days. But, I have to admit that this has been a difficult situation for me to focus on my research. Meanwhile, the outbreak, though saddening, is intriguing phenomenon for any researcher. Tons of data on the outbreak is pouring in from all over the world everyday. So, I have decided to practice some data visualization technqiues making use of the data. I will be using python language (v3.8.2) and the <a href= "https://bokeh.org/" >Bokeh library </a>, in particular, to visualize and then embed the results here. The dataset I will be working on is the COVID19 outbreak data for my home state of Tamil Nadu. The source is the <a href="https://stopcorona.tn.gov.in/">official website</a> of the Tamil Nadu health department dedicated for addressing the COVID19 outbreak. Hopefully, the source is regulary updated so that I can also regularly update the visualizations. (The plots are best viewed in a desktop)
</p>

<p>
Update: 09 April 2020
</p>
<p>
There is a major concern that India is not carrying out enough tests. The state of Tamil Nadu which has a population of 82 million has conducted a total of only 7267 tests till 09 April 2020. To get some perspective, South Korea, a country which is being praised universally for its immaculate management of the COVID19 crisis has a population of about 52 million. The tests per million (TPM) is one of the highest and is seen as key to their success by experts. Tamil Nadu crossed the 100 cases mark on 31st March 2020. From 1st April 2020 to 9th April 2020, the number of tests conducted were 4913. The low number of tests conducted in Tamil Nadu makes it difficult to say for certain the degree of tranmission within the population. Also, a majority of the tests carried out was focussed on a single source group. With the arrival of nearly 50,000 rapid antibody test kits expected soon, we will hopefully get a clearer picture in the coming days. With the increase in number of tests, plateauing or decreasing of the %positive trend would be a welcome sight.
</p>
<p>
Update: 27 April 2020
</p>
<p>
This is day 34 of the national lockdown. Although some recommendations for easing restrictions has been made by the central governemnt recently, this is not applicable for Chennai and also to pretty much the whole of Tamil Nadu because of number of zones considered as "hot spots". I have made changes to the third plot above after more clarifications emerged from the Tamil Nadu government. One of the important clarifications being the number of repeat samples now available. So, earlier I had calculated the %positive cases from the total samples collected which is inaccurate. Now, in the updated plot, %positive cases is calculated from the number of unique samples processed. The unique samples processed is obtained from subtracting the repeat samples and the samples under process from the total samples collected. I have also included the % active positive cases. This value excludes those discharged after recovery and those deceased. I will soon add more graphs visualizing other data such as recovered and deceased numbers. 
</p>
<p>
Update: 05 May 2020
</p>
<p>
There has been some relaxations in the lockdown restrictions but this is accomponied by record daily cases in India. Tamil Nadu is turning out to be a major contributor to the total national count. There are many reasons being debated non-stop in the media for the rise in the number of cases in the recent days. So, I'm not going to get into that. Back to the data visualisations, I've added another plot - the cumulative positive cases in the last 14 days for every district in Tamil Nadu. A selection menu is included for choosing the district. I was struggling  to get this plot right (it is not perfect yet) for several hours stretched over several days. I finally got it to work yesterday. 
</p>
<p>
P. S.
</p>
<p>
Apart from the official Python and Bokeh documentations and numerous google searches to check and correct minor issues in the python code, there are a few sources which helped me a lot in writing this code. I'm listing them below:
<ul>
<li>   <a href="https://stackoverflow.com/questions/49722791/python-bokeh-vbar-hover-tool"> Stackoverflow question on adding hovertool to bargraph </a> </li>

<li> <a href="https://stackoverflow.com/questions/25050311/extract-first-item-of-each-sublist"> Stack Overflow question on list comprehension </a></li>

<li> Stack Overflow questions <a href="https://stackoverflow.com/questions/25199665/one-chart-with-two-different-y-axis-ranges-in-bokeh/30914348#30914348">(1) </a><a href = "https://stackoverflow.com/questions/29267141/bokeh-add-label-to-second-axis-on-the-right">(2)</a> on adding second axis.</li>
</ul>
</p>



