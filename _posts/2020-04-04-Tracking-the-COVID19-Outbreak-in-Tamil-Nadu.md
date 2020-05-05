---
layout: post
title:  "Tracking the COVID19 outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<p>Graphs updated: 2115 hours 05 May 2020 </p>

  
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
 
   <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="64bc8010-9b93-43c3-ad2d-76a99f0f6881" data-root-id="1002"></div>
            
          
        
      
      
        <script type="application/json" id="1272">
          {"12f7a71e-ffef-4559-a7de-f26a44ef5d80":{"roots":{"references":[{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{"axis_label":"No. of Samples (in thousands)","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1044"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"label":{"value":"Processed samples"},"renderers":[{"id":"1038"}]},"id":"1047","type":"LegendItem"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null,"visible":false},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{"interval":2},"id":"1090","type":"SingleIntervalTicker"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"white"},"line_alpha":{"value":0.1},"line_color":{"value":"green"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1050","type":"Circle"},{"attributes":{"data_source":{"id":"1048"},"glyph":{"id":"1049"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1050"},"selection_glyph":null,"view":{"id":"1052"}},"id":"1051","type":"GlyphRenderer"},{"attributes":{"items":[{"id":"1047"},{"id":"1070"},{"id":"1088"}],"location":[1,164.751]},"id":"1046","type":"Legend"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"],"y":["nan","nan","0.059","0.07","0.074","0.074","0.077","0.079","0.086","0.096","0.139","0.234","0.235","0.306","0.345","0.359","0.512","0.623","0.78","0.962","1.195","1.435","1.682","1.92","2.354","2.726","2.868","3.2","3.841","4.273","4.72","5.104","5.631","6.658","7.749","8.748","9.448","11.61","14.438","16.452","20.01","22.951","28.564","33.33","39.602","45.178","51.135","58.519","64.351","71.211","79.018","84.958","91.281","99.14","109.054","118.098","129.097","139.152","152.627","164.751"]},"selected":{"id":"1068"},"selection_policy":{"id":"1069"}},"id":"1048","type":"ColumnDataSource"},{"attributes":{"fill_color":{"value":"white"},"line_color":{"value":"green"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1049","type":"Circle"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{"source":{"id":"1048"}},"id":"1052","type":"CDSView"},{"attributes":{"data_source":{"id":"1055"},"glyph":{"id":"1056"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1057"},"selection_glyph":null,"view":{"id":"1059"},"y_range_name":"foo"},"id":"1058","type":"GlyphRenderer"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["Value","@y"]]},"id":"1053","type":"HoverTool"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","1.28","0.98","1.74","1.95","1.76","2.41","2.95","3.01","3.18","2.93","2.97","3.49","5.27","8.58","10.77","12.84","12.63","13.36","13.16","13.52","13.11","12.53","11.76","11.08","11.38","10.1","8.34","7.55","6.33","5.76","4.8","4.43","3.84","3.53","3.19","2.88","2.73","2.56","2.39","2.28","2.25","2.18","2.13","2.14","2.14","2.17","2.33","2.46"]},"selected":{"id":"1086"},"selection_policy":{"id":"1087"}},"id":"1055","type":"ColumnDataSource"},{"attributes":{},"id":"1094","type":"BasicTicker"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1056","type":"Line"},{"attributes":{},"id":"1095","type":"BasicTickFormatter"},{"attributes":{"source":{"id":"1055"}},"id":"1059","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1057","type":"Line"},{"attributes":{"label":{"value":"% total positive cases"},"renderers":[{"id":"1058"}]},"id":"1070","type":"LegendItem"},{"attributes":{"line_alpha":0.75,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1036","type":"Line"},{"attributes":{"source":{"id":"1035"}},"id":"1039","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1037","type":"Line"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{},"id":"1066","type":"Selection"},{"attributes":{},"id":"1105","type":"Selection"},{"attributes":{},"id":"1067","type":"UnionRenderers"},{"attributes":{},"id":"1106","type":"UnionRenderers"},{"attributes":{},"id":"1068","type":"Selection"},{"attributes":{},"id":"1069","type":"UnionRenderers"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1053"}]},"id":"1027","type":"Toolbar"},{"attributes":{},"id":"1042","type":"CategoricalTickFormatter"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"],"y":["nan","nan","0.059","0.07","0.074","0.074","0.077","0.079","0.086","0.096","0.139","0.234","0.235","0.306","0.345","0.359","0.512","0.623","0.78","0.962","1.195","1.435","1.682","1.92","2.354","2.726","2.868","3.2","3.841","4.273","4.72","5.104","5.631","6.658","7.749","8.748","9.448","11.61","14.438","16.452","20.01","22.951","28.564","33.33","39.602","45.178","51.135","58.519","64.351","71.211","79.018","84.958","91.281","99.14","109.054","118.098","129.097","139.152","152.627","164.751"]},"selected":{"id":"1066"},"selection_policy":{"id":"1067"}},"id":"1035","type":"ColumnDataSource"},{"attributes":{"line_alpha":0.75,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1072","type":"Line"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","0.85","0.65","1.45","1.67","1.56","2.25","2.69","2.81","3.01","2.72","2.79","3.13","4.97","8.33","10.5","12.59","12.34","13.06","12.86","13.01","12.59","12","11.07","10.46","10.73","9.48","7.67","6.73","5.34","4.45","3.46","3.14","2.63","2.08","1.85","1.55","1.34","1.17","1.06","0.95","0.98","0.93","0.95","1","1.07","1.16","1.38","1.54"]},"selected":{"id":"1105"},"selection_policy":{"id":"1106"}},"id":"1071","type":"ColumnDataSource"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1095"},"major_label_text_font_size":"10pt","ticker":{"id":"1094"},"y_range_name":"foo"},"id":"1089","type":"LinearAxis"},{"attributes":{"data_source":{"id":"1071"},"glyph":{"id":"1072"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1073"},"selection_glyph":null,"view":{"id":"1075"},"y_range_name":"foo"},"id":"1074","type":"GlyphRenderer"},{"attributes":{"source":{"id":"1071"}},"id":"1075","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1073","type":"Line"},{"attributes":{},"id":"1086","type":"Selection"},{"attributes":{"label":{"value":"% active positive cases"},"renderers":[{"id":"1074"}]},"id":"1088","type":"LegendItem"},{"attributes":{"end":15},"id":"1034","type":"Range1d"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"},{"id":"1046"},{"id":"1001"}],"extra_y_ranges":{"foo":{"id":"1034"}},"left":[{"id":"1016"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"},{"id":"1051"},{"id":"1058"},{"id":"1074"}],"right":[{"id":"1089"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1044","type":"BasicTickFormatter"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":159.751},"id":"1001","type":"Label"},{"attributes":{"end":169.751},"id":"1007","type":"Range1d"},{"attributes":{},"id":"1087","type":"UnionRenderers"},{"attributes":{"text":"Samples processed and percentage of positive samples","text_font_size":{"value":"15pt"}},"id":"1003","type":"Title"},{"attributes":{"data_source":{"id":"1035"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"id":"1005","type":"FactorRange"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1042"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1090"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{},"id":"1011","type":"LinearScale"}],"root_ids":["1002"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1272').textContent;
                  var render_items = [{"docid":"12f7a71e-ffef-4559-a7de-f26a44ef5d80","root_ids":["1002"],"roots":{"1002":"64bc8010-9b93-43c3-ad2d-76a99f0f6881"}}];
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
 
 
 
 <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="981d22eb-cfe0-40eb-b5b0-677ada4ff631" data-root-id="1003"></div>
            
          
        
      
      
        <script type="application/json" id="1128">
          {"40253bd0-7231-471f-8288-6c83f751152a":{"roots":{"references":[{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1040"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1045"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{},"id":"1048","type":"Selection"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1042"}]},"id":"1028","type":"Toolbar"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1049","type":"UnionRenderers"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1042","type":"HoverTool"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1002"}],"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"}],"title":{"id":"1004"},"toolbar":{"id":"1028"},"x_range":{"id":"1006"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1045","type":"BasicTickFormatter"},{"attributes":{"source":{"id":"1001"}},"id":"1039","type":"CDSView"},{"attributes":{"interval":2},"id":"1040","type":"SingleIntervalTicker"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":498},"id":"1002","type":"Label"},{"attributes":{"data":{"daily_counts":["1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105","43","76","33","54","72","66","64","52","121","104","161","203","231","266","527","508"],"pos_counts":["1","1","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477","1520","1596","1629","1683","1755","1821","1885","1937","2058","2162","2323","2526","2757","3023","3550","4058"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"selected":{"id":"1048"},"selection_policy":{"id":"1049"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"20pt"}},"id":"1004","type":"Title"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1047","type":"CategoricalTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{},"id":"1012","type":"LinearScale"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{},"id":"1008","type":"DataRange1d"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"id":"1006","type":"FactorRange"}],"root_ids":["1003"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1128').textContent;
                  var render_items = [{"docid":"40253bd0-7231-471f-8288-6c83f751152a","root_ids":["1003"],"roots":{"1003":"981d22eb-cfe0-40eb-b5b0-677ada4ff631"}}];
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

  <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-widgets-2.0.1.min.js" integrity="sha384-xZlADit0Q04ISQEdKg2k3L4W9AwQBAuDs9nJL9fM/WwzL1tEU9VPNezOFX0nLEAz" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="8f67b505-ff49-4f86-b3c2-5d6d13285580" data-root-id="1043"></div>
            
          
        
      
      
        <script type="application/json" id="1132">
          {"d749f67e-56b2-4de0-8077-76adb5801730":{"roots":{"references":[{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{},"id":"1049","type":"Selection"},{"attributes":{},"id":"1050","type":"UnionRenderers"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"data":{"x":["22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"],"y":["6","6","6","6","6","6","6","6","7","8","26","28","34","34"],"y0":["6","6","6","6","6","6","6","6","7","8","26","28","34","34"],"y1":["56","57","57","58","58","58","70","73","78","86","90","93","97","136"],"y10":["16","16","16","16","16","16","16","16","16","16","16","17","17","17"],"y11":["42","42","42","42","42","42","42","42","42","43","43","43","44","44"],"y12":["0","0","0","0","0","0","0","0","0","0","0","0","0","2"],"y13":["50","52","56","60","75","79","79","79","84","87","88","90","91","91"],"y14":["44","44","44","44","44","44","44","44","44","45","45","45","45","45"],"y15":["51","55","55","55","59","59","61","61","61","61","61","61","61","76"],"y16":["9","9","9","9","9","9","9","9","9","9","9","9","9","13"],"y17":["5","5","5","7","7","7","7","7","9","9","11","11","36","37"],"y18":["1","1","1","1","1","1","1","1","1","1","1","1","1","1"],"y19":["11","12","14","14","15","15","15","15","18","18","20","20","21","21"],"y2":["373","400","452","495","523","570","673","768","906","1082","1257","1458","1724","2008"],"y20":["39","39","39","39","39","39","39","39","40","40","40","40","43","43"],"y21":["24","29","30","30","31","31","31","31","32","32","33","33","33","34"],"y22":["12","12","12","12","12","12","12","12","12","12","12","12","12","12"],"y23":["31","32","33","38","38","38","38","38","38","38","38","40","49","50"],"y24":["54","55","55","55","55","55","55","55","55","57","57","57","58","58"],"y25":["43","43","43","43","43","43","43","43","43","43","44","44","44","49"],"y26":["62","63","63","63","63","63","63","63","63","63","63","63","63","19"],"y27":["17","18","18","18","18","18","18","18","18","18","18","18","19","95"],"y28":["109","110","110","110","112","112","112","112","112","112","114","114","114","25"],"y29":["50","50","52","52","53","53","53","54","55","61","68","70","79","31"],"y3":["134","134","141","141","141","141","141","141","141","141","142","146","146","146"],"y30":["13","13","14","15","15","15","15","15","15","15","15","16","27","27"],"y31":["28","29","29","29","29","29","29","29","29","29","29","29","31","64"],"y32":["51","51","51","51","51","51","51","51","51","51","51","51","55","114"],"y33":["27","27","27","27","27","27","27","27","27","27","27","27","27","56"],"y34":["22","22","22","22","22","22","22","22","22","22","22","22","22","22"],"y35":["41","42","42","43","47","48","48","50","50","51","53","86","135","159"],"y36":["19","22","23","25","32","32","32","32","32","32","32","32","34","35"],"y4":["26","26","26","26","26","26","26","26","27","28","30","39","161","229"],"y5":["0","1","1","1","1","1","1","1","1","1","1","1","1","2"],"y6":["77","80","80","80","80","80","80","80","80","81","81","81","91","98"],"y7":["70","70","70","70","70","70","70","70","70","70","70","70","70","70"],"y8":["5","5","5","5","6","6","9","9","9","9","9","15","15","53"],"y9":["11","11","12","19","19","19","20","23","26","28","41","41","41","42"]},"selected":{"id":"1049"},"selection_policy":{"id":"1050"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"js_property_callbacks":{"change:value":[{"id":"1041"}]},"options":["Ariyalur","Chengalpattu","Chennai","Coimbatore","Cuddalore","Dharmapuri","Dindigul","Erode","Kallakurichi","Kancheepuram","Kanyakumari","Karur","Krishnagiri","Madurai","Nagapattinam","Namakkal","Nilgiris","Perambalur","Pudukottai","Ramnad","Ranipet","Salem","Sivagangai","Tenkasi","Thanjavur","Theni","Tirunelveli","Tirupathur","Tiruppur","Tiruvallur","Tiruvannamalai","Tiruvarur","Trichy","Tuticorin","Vellore","Villupuram","Virudhunagar"],"title":"Select District:","value":"Ariyalur","width":150},"id":"1042","type":"Select"},{"attributes":{"children":[{"id":"1042"},{"id":"1002"}]},"id":"1043","type":"Row"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"args":{"source":{"id":"1001"}},"code":"\n        var data = source.data;\n        var f = cb_obj.value\n        if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Chengalpattu\") {source.data['y'] = source.data['y1'];}\n        else if(f==\"Chennai\") {source.data['y'] = source.data['y2'];}\n        else if(f==\"Coimbatore\") {source.data['y'] = source.data['y3'];}\n        else if(f==\"Cuddalore\") {source.data['y'] = source.data['y4'];}\n        else if(f==\"Dharmapuri\") {source.data['y'] = source.data['y5'];}\n        else if(f==\"Dindigul\") {source.data['y'] = source.data['y6'];}\n        else if(f==\"Erode\") {source.data['y'] = source.data['y7'];}\n        else if(f==\"Kallakurichi\") {source.data['y'] = source.data['y8'];}\n        else if(f==\"Kancheepuram\") {source.data['y'] = source.data['y9'];}\n        else if(f==\"Kanyakumari\") {source.data['y'] = source.data['y10'];}\n        else if(f==\"Karur\") {source.data['y'] = source.data['y11'];}\n        else if(f==\"Krishnagiri\") {source.data['y'] = source.data['y12'];}\n        else if(f==\"Madurai\") {source.data['y'] = source.data['y13'];}\n        else if(f==\"Nagapattinam\") {source.data['y'] = source.data['y14'];}\n        else if(f==\"Namakkal\") {source.data['y'] = source.data['y15'];}\n        else if(f==\"Nilgiris\") {source.data['y'] = source.data['y16'];}\n        else if(f==\"Perambalur\") {source.data['y'] = source.data['y17'];}\n        else if(f==\"Pudukottai\") {source.data['y'] = source.data['y18'];}\n        else if(f==\"Ramnad\") {source.data['y'] = source.data['y19'];}\n        else if(f==\"Ranipet\") {source.data['y'] = source.data['y20'];}\n        else if(f==\"Salem\") {source.data['y'] = source.data['y21'];}\n        else if(f==\"Sivagangai\") {source.data['y'] = source.data['y22'];}\n        else if(f==\"Tenkasi\") {source.data['y'] = source.data['y23'];}\n        else if(f==\"Thanjavur\") {source.data['y'] = source.data['y24'];}\n        else if(f==\"Theni\") {source.data['y'] = source.data['y25'];}\n        else if(f==\"Tirunelveli\") {source.data['y'] = source.data['y26'];}\n        else if(f==\"Tirupathur\") {source.data['y'] = source.data['y27'];}\n        else if(f==\"Tiruppur\") {source.data['y'] = source.data['y28'];}\n        else if(f==\"Tiruvallur\") {source.data['y'] = source.data['y29'];}\n        else if(f==\"Tiruvannamalai\") {source.data['y'] = source.data['y30'];}\n        else if(f==\"Tiruvarur\") {source.data['y'] = source.data['y31'];}\n        else if(f==\"Trichy\") {source.data['y'] = source.data['y32'];}\n        else if(f==\"Tuticorin\") {source.data['y'] = source.data['y33'];}\n        else if(f==\"Vellore\") {source.data['y'] = source.data['y34'];}\n        else if(f==\"Villupuram\") {source.data['y'] = source.data['y35'];}\n        else if(f==\"Virudhunagar\") {source.data['y'] = source.data['y36'];}\n        source.change.emit();\n\n    "},"id":"1041","type":"CustomJS"},{"attributes":{"source":{"id":"1001"}},"id":"1038","type":"CDSView"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1039"}]},"id":"1027","type":"Toolbar"},{"attributes":{},"id":"1045","type":"CategoricalTickFormatter"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@y"]]},"id":"1039","type":"HoverTool"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"}],"left":[{"id":"1016"}],"plot_height":350,"plot_width":550,"renderers":[{"id":"1037"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1014","type":"CategoricalTicker"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"text":"Number of positive cases (Cumulative) in the last 14 days"},"id":"1003","type":"Title"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1045"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1014"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1007","type":"DataRange1d"},{"attributes":{"factors":["22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"id":"1005","type":"FactorRange"},{"attributes":{},"id":"1047","type":"BasicTickFormatter"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{},"id":"1011","type":"LinearScale"}],"root_ids":["1043"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1132').textContent;
                  var render_items = [{"docid":"d749f67e-56b2-4de0-8077-76adb5801730","root_ids":["1043"],"roots":{"1043":"8f67b505-ff49-4f86-b3c2-5d6d13285580"}}];
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

<head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="981d22eb-cfe0-40eb-b5b0-677ada4ff631" data-root-id="1003"></div>
            
          
        
      
      
        <script type="application/json" id="1128">
          {"40253bd0-7231-471f-8288-6c83f751152a":{"roots":{"references":[{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1040"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1045"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{},"id":"1048","type":"Selection"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1042"}]},"id":"1028","type":"Toolbar"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1049","type":"UnionRenderers"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1042","type":"HoverTool"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1002"}],"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"}],"title":{"id":"1004"},"toolbar":{"id":"1028"},"x_range":{"id":"1006"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1045","type":"BasicTickFormatter"},{"attributes":{"source":{"id":"1001"}},"id":"1039","type":"CDSView"},{"attributes":{"interval":2},"id":"1040","type":"SingleIntervalTicker"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":498},"id":"1002","type":"Label"},{"attributes":{"data":{"daily_counts":["1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105","43","76","33","54","72","66","64","52","121","104","161","203","231","266","527","508"],"pos_counts":["1","1","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477","1520","1596","1629","1683","1755","1821","1885","1937","2058","2162","2323","2526","2757","3023","3550","4058"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"selected":{"id":"1048"},"selection_policy":{"id":"1049"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"20pt"}},"id":"1004","type":"Title"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1047","type":"CategoricalTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{},"id":"1012","type":"LinearScale"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{},"id":"1008","type":"DataRange1d"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May"]},"id":"1006","type":"FactorRange"}],"root_ids":["1003"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1128').textContent;
                  var render_items = [{"docid":"40253bd0-7231-471f-8288-6c83f751152a","root_ids":["1003"],"roots":{"1003":"981d22eb-cfe0-40eb-b5b0-677ada4ff631"}}];
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



