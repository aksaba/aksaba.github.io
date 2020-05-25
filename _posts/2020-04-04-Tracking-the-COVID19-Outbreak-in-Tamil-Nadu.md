---
layout: post
title:  "Tracking the COVID19 outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<p>Graphs updated: 2030 hours 25 May 2020 </p>

  <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="a891f79a-bf17-4b8f-8119-7291b87d20f7" data-root-id="1086"></div>
            
          
        
      
      
        <script type="application/json" id="1233">
          {"fb9df520-5942-4dff-a792-fd56cfd9b2b5":{"roots":{"references":[{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":785},"id":"1044","type":"Label"},{"attributes":{},"id":"1093","type":"BasicTickFormatter"},{"attributes":{},"id":"1050","type":"DataRange1d"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1090"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1069","type":"BoxAnnotation"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"15pt"}},"id":"1046","type":"Title"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{"source":{"id":"1001"}},"id":"1039","type":"CDSView"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"below":[{"id":"1056"}],"center":[{"id":"1058"},{"id":"1062"},{"id":"1044"}],"left":[{"id":"1059"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1080"}],"title":{"id":"1046"},"toolbar":{"id":"1070"},"x_range":{"id":"1048"},"x_scale":{"id":"1052"},"y_range":{"id":"1050"},"y_scale":{"id":"1054"}},"id":"1045","subtype":"Figure","type":"Plot"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@pos_counts"]]},"id":"1042","type":"HoverTool"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1094"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1082"}},"id":"1056","type":"CategoricalAxis"},{"attributes":{"interval":2},"id":"1082","type":"SingleIntervalTicker"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"id":"1048","type":"FactorRange"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1063"},{"id":"1064"},{"id":"1065"},{"id":"1066"},{"id":"1067"},{"id":"1068"},{"id":"1084"}]},"id":"1070","type":"Toolbar"},{"attributes":{},"id":"1063","type":"PanTool"},{"attributes":{},"id":"1096","type":"Selection"},{"attributes":{},"id":"1097","type":"UnionRenderers"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1078","type":"VBar"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{"source":{"id":"1001"}},"id":"1081","type":"CDSView"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1079","type":"VBar"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1078"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1079"},"selection_glyph":null,"view":{"id":"1081"}},"id":"1080","type":"GlyphRenderer"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1084","type":"HoverTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1042"}]},"id":"1028","type":"Toolbar"},{"attributes":{"data":{"daily_counts":["1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105","43","76","33","54","72","66","64","52","121","104","161","203","231","266","527","508","771","580","600","526","669","798","716","509","447","434","477","639","536","688","743","776","786","759","765","805"],"pos_counts":["1","1","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477","1520","1596","1629","1683","1755","1821","1885","1937","2058","2162","2323","2526","2757","3023","3550","4058","4829","5409","6009","6535","7204","8002","8718","9227","9674","10108","10585","11224","11760","12448","13191","13967","14753","15512","16277","17082"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"selected":{"id":"1096"},"selection_policy":{"id":"1097"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"axis":{"id":"1056"},"ticker":null},"id":"1058","type":"Grid"},{"attributes":{},"id":"1090","type":"BasicTickFormatter"},{"attributes":{"children":[{"id":"1004"},{"id":"1045"}]},"id":"1086","type":"Column"},{"attributes":{},"id":"1052","type":"CategoricalScale"},{"attributes":{},"id":"1091","type":"CategoricalTickFormatter"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1093"},"major_label_text_font_size":"10pt","ticker":{"id":"1060"}},"id":"1059","type":"LinearAxis"},{"attributes":{},"id":"1054","type":"LinearScale"},{"attributes":{},"id":"1060","type":"BasicTicker"},{"attributes":{"axis":{"id":"1059"},"dimension":1,"ticker":null},"id":"1062","type":"Grid"},{"attributes":{},"id":"1094","type":"CategoricalTickFormatter"},{"attributes":{},"id":"1064","type":"WheelZoomTool"},{"attributes":{},"id":"1068","type":"HelpTool"},{"attributes":{"overlay":{"id":"1069"}},"id":"1065","type":"BoxZoomTool"},{"attributes":{},"id":"1066","type":"SaveTool"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":16482},"id":"1002","type":"Label"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1002"}],"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"}],"title":{"id":"1005"},"toolbar":{"id":"1028"},"x_range":{"id":"1003"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1004","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1067","type":"ResetTool"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"id":"1003","type":"FactorRange"},{"attributes":{"text":"Number of positive cases (Cumulative)","text_font_size":{"value":"15pt"}},"id":"1005","type":"Title"},{"attributes":{"interval":2},"id":"1040","type":"SingleIntervalTicker"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1091"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1040"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{},"id":"1012","type":"LinearScale"},{"attributes":{},"id":"1008","type":"DataRange1d"}],"root_ids":["1086"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1233').textContent;
                  var render_items = [{"docid":"fb9df520-5942-4dff-a792-fd56cfd9b2b5","root_ids":["1086"],"roots":{"1086":"a891f79a-bf17-4b8f-8119-7291b87d20f7"}}];
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
<hr>
<head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="93af99c7-c326-4f58-98c1-aa9fb5564f90" data-root-id="1002"></div>
            
          
        
      
      
        <script type="application/json" id="1239">
          {"e201dbf2-b193-4ae1-a1a3-2d7851c1b904":{"roots":{"references":[{"attributes":{},"id":"1042","type":"BasicTickFormatter"},{"attributes":{"axis_label":"No. of Samples (in thousands)","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1042"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"label":{"value":"Processed samples"},"renderers":[{"id":"1038"}]},"id":"1047","type":"LegendItem"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null,"visible":false},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","1.28","0.98","1.74","1.95","1.76","2.41","2.95","3.01","3.18","2.93","2.97","3.49","5.27","8.58","10.77","12.84","12.63","13.36","13.16","13.52","13.11","12.53","11.76","11.08","11.38","10.1","8.34","7.55","6.33","5.76","4.8","4.43","3.84","3.53","3.19","2.88","2.73","2.56","2.39","2.28","2.25","2.18","2.13","2.14","2.14","2.17","2.33","2.46","2.72","2.83","2.92","2.99","3.11","3.3","3.43","3.45","3.46","3.49","3.54","3.56","3.65","3.76","3.84","3.93","4.02","4.09","4.17","4.25"]},"selected":{"id":"1078"},"selection_policy":{"id":"1077"}},"id":"1050","type":"ColumnDataSource"},{"attributes":{"data_source":{"id":"1050"},"glyph":{"id":"1051"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1052"},"selection_glyph":null,"view":{"id":"1054"},"y_range_name":"foo"},"id":"1053","type":"GlyphRenderer"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1094","type":"UnionRenderers"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["Value","@y"]]},"id":"1048","type":"HoverTool"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"id":"1005","type":"FactorRange"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{"source":{"id":"1050"}},"id":"1054","type":"CDSView"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1052","type":"Line"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"label":{"value":"% total positive cases"},"renderers":[{"id":"1053"}]},"id":"1063","type":"LegendItem"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1051","type":"Line"},{"attributes":{},"id":"1095","type":"Selection"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":382.074},"id":"1001","type":"Label"},{"attributes":{},"id":"1061","type":"UnionRenderers"},{"attributes":{"line_alpha":0.1,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1037","type":"Line"},{"attributes":{},"id":"1062","type":"Selection"},{"attributes":{"items":[{"id":"1047"},{"id":"1063"},{"id":"1079"}],"location":[1,162.074]},"id":"1046","type":"Legend"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"line_alpha":0.75,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1065","type":"Line"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","0.85","0.65","1.45","1.67","1.56","2.25","2.69","2.81","3.01","2.72","2.79","3.13","4.97","8.33","10.5","12.59","12.34","13.06","12.86","13.01","12.59","12","11.07","10.46","10.73","9.48","7.67","6.73","5.34","4.45","3.46","3.14","2.63","2.08","1.85","1.55","1.34","1.17","1.06","0.95","0.98","0.93","0.95","1","1.07","1.16","1.38","1.54","1.84","2","2.12","2.13","2.24","2.43","2.56","2.61","2.64","2.56","2.33","2.21","2.26","2.25","2.1","2.14","2.05","2.09","2.01","2.05"]},"selected":{"id":"1095"},"selection_policy":{"id":"1094"}},"id":"1064","type":"ColumnDataSource"},{"attributes":{"data_source":{"id":"1064"},"glyph":{"id":"1065"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1066"},"selection_glyph":null,"view":{"id":"1068"},"y_range_name":"foo"},"id":"1067","type":"GlyphRenderer"},{"attributes":{"source":{"id":"1064"}},"id":"1068","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1066","type":"Line"},{"attributes":{"label":{"value":"% active positive cases"},"renderers":[{"id":"1067"}]},"id":"1079","type":"LegendItem"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1048"}]},"id":"1027","type":"Toolbar"},{"attributes":{},"id":"1077","type":"UnionRenderers"},{"attributes":{},"id":"1078","type":"Selection"},{"attributes":{"source":{"id":"1035"}},"id":"1039","type":"CDSView"},{"attributes":{"line_alpha":0.75,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1036","type":"Line"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"],"y":["nan","nan","0.059","0.07","0.074","0.074","0.077","0.079","0.086","0.096","0.139","0.234","0.235","0.306","0.345","0.359","0.512","0.623","0.78","0.962","1.195","1.435","1.682","1.92","2.354","2.726","2.868","3.2","3.841","4.273","4.72","5.104","5.631","6.658","7.749","8.748","9.448","11.61","14.438","16.452","20.01","22.951","28.564","33.33","39.602","45.178","51.135","58.519","64.351","71.211","79.018","84.958","91.281","99.14","109.054","118.098","129.097","139.152","152.627","164.751","177.601","191.378","205.495","218.847","231.692","242.617","254.335","267.768","279.266","289.955","298.645","315.026","321.973","331.465","343.227","355.226","367.436","379.199","390.604","402.074"]},"selected":{"id":"1062"},"selection_policy":{"id":"1061"}},"id":"1035","type":"ColumnDataSource"},{"attributes":{},"id":"1044","type":"CategoricalTickFormatter"},{"attributes":{"interval":2},"id":"1081","type":"SingleIntervalTicker"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1085"},"major_label_text_font_size":"10pt","ticker":{"id":"1084"},"y_range_name":"foo"},"id":"1080","type":"LinearAxis"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"},{"id":"1046"},{"id":"1001"}],"extra_y_ranges":{"foo":{"id":"1034"}},"left":[{"id":"1016"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"},{"id":"1053"},{"id":"1067"}],"right":[{"id":"1080"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{"text":"Samples processed and percentage of positive samples","text_font_size":{"value":"15pt"}},"id":"1003","type":"Title"},{"attributes":{"end":15},"id":"1034","type":"Range1d"},{"attributes":{"data_source":{"id":"1035"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{},"id":"1084","type":"BasicTicker"},{"attributes":{},"id":"1085","type":"BasicTickFormatter"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{"end":407.074},"id":"1007","type":"Range1d"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1044"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1081"}},"id":"1013","type":"CategoricalAxis"}],"root_ids":["1002"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1239').textContent;
                  var render_items = [{"docid":"e201dbf2-b193-4ae1-a1a3-2d7851c1b904","root_ids":["1002"],"roots":{"1002":"93af99c7-c326-4f58-98c1-aa9fb5564f90"}}];
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
<hr>
  <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="3f0cb91b-d7e4-4a72-8def-24818033dbba" data-root-id="1003"></div>
            
          
        
      
      
        <script type="application/json" id="1193">
          {"330b68df-7d9f-41e9-8473-6e5c1e07e90b":{"roots":{"references":[{"attributes":{},"id":"1050","type":"BasicTickFormatter"},{"attributes":{"items":[{"id":"1055"}],"location":[1,268.0]},"id":"1054","type":"Legend"},{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"axis_label":"Count","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1050"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"source":{"id":"1041"}},"id":"1045","type":"CDSView"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1052","type":"Selection"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1037"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1038"},"selection_glyph":null,"view":{"id":"1040"}},"id":"1039","type":"GlyphRenderer"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1053","type":"UnionRenderers"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1043","type":"Line"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1042","type":"Line"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"],"y":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","4.35","3.45","2.63","2.38","2","1.49","0.81","0.43","0.32","0.24","0.62","0.88","0.97","1.01","1.08","0.96","0.99","1.03","1.02","0.94","1","1.13","1.18","1.13","1.09","1.02","1.12","1.13","1.1","1.19","1.25","1.26","1.27","1.24","1.21","1.25","1.16","1.11","1.05","0.99","0.87","0.81","0.72","0.68","0.67","0.67","0.65","0.66","0.7","0.69","0.68","0.7","0.7","0.69","0.69","0.67","0.66","0.67","0.66","0.66","0.68","0.69"]},"selected":{"id":"1070"},"selection_policy":{"id":"1071"}},"id":"1041","type":"ColumnDataSource"},{"attributes":{"source":{"id":"1001"}},"id":"1040","type":"CDSView"},{"attributes":{"label":{"value":"% mortality rate"},"renderers":[{"id":"1044"}]},"id":"1055","type":"LegendItem"},{"attributes":{"interval":2},"id":"1057","type":"SingleIntervalTicker"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of deaths","@death_counts"],["% mortality","@death_percent"]]},"id":"1059","type":"HoverTool"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1063"},"major_label_text_font_size":"10pt","ticker":{"id":"1062"},"y_range_name":"foo"},"id":"1056","type":"LinearAxis"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{},"id":"1062","type":"BasicTicker"},{"attributes":{},"id":"1063","type":"BasicTickFormatter"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1059"}]},"id":"1028","type":"Toolbar"},{"attributes":{"data":{"death_counts":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","1","1","1","1","1","1","1","1","1","1","3","5","6","7","8","8","9","10","11","11","12","14","15","15","15","15","17","18","18","20","22","23","24","24","25","27","27","28","29","30","31","33","35","37","40","44","47","53","61","64","66","71","74","78","81","84","87","94","98","103","111","118"],"death_percent":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","4.35","3.45","2.63","2.38","2","1.49","0.81","0.43","0.32","0.24","0.62","0.88","0.97","1.01","1.08","0.96","0.99","1.03","1.02","0.94","1","1.13","1.18","1.13","1.09","1.02","1.12","1.13","1.1","1.19","1.25","1.26","1.27","1.24","1.21","1.25","1.16","1.11","1.05","0.99","0.87","0.81","0.72","0.68","0.67","0.67","0.65","0.66","0.7","0.69","0.68","0.7","0.7","0.69","0.69","0.67","0.66","0.67","0.66","0.66","0.68","0.69"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"selected":{"id":"1052"},"selection_policy":{"id":"1053"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"death_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1038","type":"VBar"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"death_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1070","type":"Selection"},{"attributes":{},"id":"1071","type":"UnionRenderers"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":113},"id":"1002","type":"Label"},{"attributes":{"text":"Number of deaths (Cumulative) and % mortality rate","text_font_size":{"value":"15pt"}},"id":"1004","type":"Title"},{"attributes":{"end":5},"id":"1035","type":"Range1d"},{"attributes":{},"id":"1048","type":"CategoricalTickFormatter"},{"attributes":{"data_source":{"id":"1041"},"glyph":{"id":"1042"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1043"},"selection_glyph":null,"view":{"id":"1045"},"y_range_name":"foo"},"id":"1044","type":"GlyphRenderer"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1054"},{"id":"1002"}],"extra_y_ranges":{"foo":{"id":"1035"}},"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1039"},{"id":"1044"}],"right":[{"id":"1056"}],"title":{"id":"1004"},"toolbar":{"id":"1028"},"x_range":{"id":"1006"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","43975","43976"]},"id":"1006","type":"FactorRange"},{"attributes":{"end":123},"id":"1008","type":"Range1d"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1048"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1057"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{},"id":"1012","type":"LinearScale"}],"root_ids":["1003"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1193').textContent;
                  var render_items = [{"docid":"330b68df-7d9f-41e9-8473-6e5c1e07e90b","root_ids":["1003"],"roots":{"1003":"3f0cb91b-d7e4-4a72-8def-24818033dbba"}}];
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
<hr>
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
    
      
        
          
          
            
              <div class="bk-root" id="d279557d-55af-4fe7-8fbe-800a5c63ee45" data-root-id="1043"></div>
            
          
        
      
      
        <script type="application/json" id="1132">
          {"524e7471-727a-4b5f-8727-a953be9831f4":{"roots":{"references":[{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{"js_property_callbacks":{"change:value":[{"id":"1041"}]},"options":["Ariyalur","Chengalpattu","Chennai","Coimbatore","Cuddalore","Dharmapuri","Dindigul","Erode","Kallakurichi","Kancheepuram","Kanyakumari","Karur","Krishnagiri","Madurai","Nagapattinam","Namakkal","Nilgiris","Perambalur","Pudukottai","Ramnad","Ranipet","Salem","Sivagangai","Tenkasi","Thanjavur","Theni","Thirupathur","Thiruvallur","Thiruvannamalai","Thiruvarur","Thoothukudi","Tirunelveli","Tiruppur","Trichy","Vellore","Villupuram","Virudhunagar"],"title":"Select District:","value":"Ariyalur","width":140},"id":"1042","type":"Select"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{},"id":"1047","type":"BasicTickFormatter"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1049","type":"Selection"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{},"id":"1050","type":"UnionRenderers"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"data":{"x":["05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May"],"y":["28","216","240","240","265","269","302","334","335","335","153","34","25","27","10","10","7","7","7","8","8"],"y0":["28","216","240","240","265","269","302","334","335","335","153","34","25","27","10","10","7","7","7","8","8"],"y1":["84","93","106","131","169","206","286","320","345","358","377","389","306","344","365","423","416","455","481","518","568"],"y10":["4","4","4","9","8","8","8","9","9","14","18","20","20","27","32","28","25","24","21","23","26"],"y11":["2","3","5","5","5","6","6","10","12","13","12","11","27","28","34","27","25","25","25","25","14"],"y12":["0","4","8","10","10","20","20","20","20","20","20","18","20","20","2","3","3","4","3","3","4"],"y13":["46","61","55","57","41","42","46","46","38","47","54","56","51","53","53","62","80","111","111","114","111"],"y14":["1","1","1","1","1","1","1","1","3","3","3","4","5","5","6","6","6","5","3","3","3"],"y15":["26","25","25","21","22","21","21","16","16","16","0","0","0","0","0","","0","0","0","0","0"],"y16":["4","4","4","4","3","3","3","3","3","3","3","3","3","3","3","2","2","2","1","1","1"],"y17":["33","36","69","68","90","99","98","124","125","124","109","109","106","106","48","48","26","6","5","4","4"],"y18":["0","3","4","4","4","5","5","5","5","5","5","5","5","5","5","7","8","11","12","13","13"],"y19":["10","9","9","10","9","10","14","14","14","9","9","9","9","15","17","17","17","25","25","28","33"],"y2":["1668","1975","2281","2644","2757","3171","3632","4093","4470","4834","5114","5017","5220","5460","5691","5345","5681","5523","5865","5653","5911"],"y20":["9","6","13","13","21","27","28","37","35","35","36","39","35","37","38","26","28","29","29","25","28"],"y21":["10","11","11","7","7","6","6","5","5","5","0","0","9","14","14","14","14","14","17","17","23"],"y22":["0","0","0","0","0","0","0","0","0","1","1","10","14","14","14","13","16","16","3","4","4"],"y23":["38","39","36","36","36","31","31","23","21","20","22","26","24","30","28","27","33","32","33","33","33"],"y24":["15","20","22","21","21","19","22","22","23","23","18","18","10","10","9","10","14","14","13","16","17"],"y25":["6","8","11","12","13","16","16","23","28","29","35","35","35","44","45","47","51","49","50","50","52"],"y26":["2","3","5","6","9","10","10","10","10","10","10","0","8","9","7","7","4","4","4","4","4"],"y27":["46","79","141","216","228","272","374","398","406","410","429","348","363","382","380","395","413","424","426","452","429"],"y28":["15","32","49","57","70","69","79","92","115","123","126","133","110","114","114","116","109","98","103","107","148"],"y29":["7","6","5","5","4","3","3","3","3","3","3","3","3","3","2","2","0","3","3","5","6"],"y3":["4","4","4","4","4","4","4","4","0","0","0","0","0","0","0","1","0","0","0","0","0"],"y30":["1","2","3","3","3","3","6","8","9","11","20","28","40","55","60","82","104","108","111","119","129"],"y31":["6","7","10","13","21","27","27","30","35","51","72","116","129","141","155","163","164","177","187","182","197"],"y32":["2","2","2","2","2","2","2","0","0","0","0","0","0","0","0","","0","0","0","0","0"],"y33":["9","10","11","12","14","14","14","12","11","11","11","10","5","5","6","2","2","6","6","9","9"],"y34":["5","11","12","11","11","14","14","15","13","13","13","12","11","11","7","7","6","9","5","5","5"],"y35":["128","133","171","192","256","255","248","244","251","251","176","153","30","34","31","38","26","24","24","24","24"],"y36":["16","13","11","14","6","8","9","13","13","12","14","13","16","17","18","24","29","52","53","54","71"],"y4":["203","298","330","364","367","368","367","367","384","384","378","164","157","55","42","38","19","15","15","17","12"],"y5":["0","2","2","3","3","3","5","4","4","4","4","4","3","1","1","1","1","0","0","0","1"],"y6":["24","31","31","27","28","28","29","31","31","31","30","25","23","25","19","20","25","26","26","22","22"],"y7":["1","0","0","0","0","0","0","0","0","0","0","0","0","0","0","1","0","1","1","1","1"],"y8":["50","49","54","54","55","54","54","51","51","51","47","64","56","61","67","54","62","60","60","75","67"],"y9":["31","75","77","85","101","101","105","129","132","97","104","81","78","95","87","98","106","98","108","132","138"]},"selected":{"id":"1049"},"selection_policy":{"id":"1050"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"args":{"source":{"id":"1001"}},"code":"\n        var data = source.data;\n        var f = cb_obj.value\n        if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Chengalpattu\") {source.data['y'] = source.data['y1'];}\n        else if(f==\"Chennai\") {source.data['y'] = source.data['y2'];}\n        else if(f==\"Coimbatore\") {source.data['y'] = source.data['y3'];}\n        else if(f==\"Cuddalore\") {source.data['y'] = source.data['y4'];}\n        else if(f==\"Dharmapuri\") {source.data['y'] = source.data['y5'];}\n        else if(f==\"Dindigul\") {source.data['y'] = source.data['y6'];}\n        else if(f==\"Erode\") {source.data['y'] = source.data['y7'];}\n        else if(f==\"Kallakurichi\") {source.data['y'] = source.data['y8'];}\n        else if(f==\"Kancheepuram\") {source.data['y'] = source.data['y9'];}\n        else if(f==\"Kanyakumari\") {source.data['y'] = source.data['y10'];}\n        else if(f==\"Karur\") {source.data['y'] = source.data['y11'];}\n        else if(f==\"Krishnagiri\") {source.data['y'] = source.data['y12'];}\n        else if(f==\"Madurai\") {source.data['y'] = source.data['y13'];}\n        else if(f==\"Nagapattinam\") {source.data['y'] = source.data['y14'];}\n        else if(f==\"Namakkal\") {source.data['y'] = source.data['y15'];}\n        else if(f==\"Nilgiris\") {source.data['y'] = source.data['y16'];}\n        else if(f==\"Perambalur\") {source.data['y'] = source.data['y17'];}\n        else if(f==\"Pudukottai\") {source.data['y'] = source.data['y18'];}\n        else if(f==\"Ramnad\") {source.data['y'] = source.data['y19'];}\n        else if(f==\"Ranipet\") {source.data['y'] = source.data['y20'];}\n        else if(f==\"Salem\") {source.data['y'] = source.data['y21'];}\n        else if(f==\"Sivagangai\") {source.data['y'] = source.data['y22'];}\n        else if(f==\"Tenkasi\") {source.data['y'] = source.data['y23'];}\n        else if(f==\"Thanjavur\") {source.data['y'] = source.data['y24'];}\n        else if(f==\"Theni\") {source.data['y'] = source.data['y25'];}\n        else if(f==\"Thirupathur\") {source.data['y'] = source.data['y26'];}\n        else if(f==\"Thiruvallur\") {source.data['y'] = source.data['y27'];}\n        else if(f==\"Thiruvannamalai\") {source.data['y'] = source.data['y28'];}\n        else if(f==\"Thiruvarur\") {source.data['y'] = source.data['y29'];}\n        else if(f==\"Thoothukudi\") {source.data['y'] = source.data['y30'];}\n        else if(f==\"Tirunelveli\") {source.data['y'] = source.data['y31'];}\n        else if(f==\"Tiruppur\") {source.data['y'] = source.data['y32'];}\n        else if(f==\"Trichy\") {source.data['y'] = source.data['y33'];}\n        else if(f==\"Vellore\") {source.data['y'] = source.data['y34'];}\n        else if(f==\"Villupuram\") {source.data['y'] = source.data['y35'];}\n        else if(f==\"Virudhunagar\") {source.data['y'] = source.data['y36'];}\n        source.change.emit();\n\n    "},"id":"1041","type":"CustomJS"},{"attributes":{"children":[{"id":"1042"},{"id":"1002"}]},"id":"1043","type":"Row"},{"attributes":{"source":{"id":"1001"}},"id":"1038","type":"CDSView"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1039"}]},"id":"1027","type":"Toolbar"},{"attributes":{},"id":"1045","type":"CategoricalTickFormatter"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"}],"left":[{"id":"1016"}],"plot_height":350,"plot_width":550,"renderers":[{"id":"1037"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@y"]]},"id":"1039","type":"HoverTool"},{"attributes":{"text":"Number of active cases in the last 21 days","text_font_size":{"value":"12pt"}},"id":"1003","type":"Title"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{},"id":"1014","type":"CategoricalTicker"},{"attributes":{"factors":["05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May"]},"id":"1005","type":"FactorRange"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1045"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1014"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1007","type":"DataRange1d"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"}],"root_ids":["1043"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1132').textContent;
                  var render_items = [{"docid":"524e7471-727a-4b5f-8727-a953be9831f4","root_ids":["1043"],"roots":{"1043":"d279557d-55af-4fe7-8fbe-800a5c63ee45"}}];
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
<hr>
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
Update: 07 May 2020
</p>
<p>
I have added the death statistics and % mortality plot. Also, I have expanded the district wise trends graph to include the last 21 days total cases. This is in accordance to the the stipulated 21 day duration prescibed by the central government for a district to move from "orange" zone to "green" zone if no new cases are reported in this period.
</p>
<p>
Update: 23 May 2020
</p>
<p>
I have updated the plots after nearly ten days.  I was a little busy writing my thesis. A lot has happened in this period. More restrictions are lifted and people stuck during the lockdown are returning to their homes via special trains and planes. As for the outbreak itself, it is almost becoming an afterthough in peoples' minds. But the reality is anything but as the number of cases is rapidly increasing in India as well as in Tamil Nadu. Looking at the data, there was a slight wobble in the number of tests because there was a brief reduction in the tests conducted for a couple of days (around 8K-10K) and then it went to be previous numbers (around 12K tests). Experts are crying out for ramping up testing but it is not happening. The gap between %total positive and %total active is increasing mainly due to revised discharge guidelines released by ICMR which has lessened the stringency of discharge criterion.  Today (23 May 2020), the number of deaths went past 100 but the %mortality has plateaued to about 0.65%.
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



