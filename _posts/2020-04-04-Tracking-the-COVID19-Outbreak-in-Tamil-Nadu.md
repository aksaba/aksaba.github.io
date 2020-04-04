---
layout: post
title:  "Tracking the COVID19 Outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<div style="text-align:justify">
<p>
This is day 10 of the lock down which is in effect because of the worldwide COVID19 outbreak. I'm in the last stretch of my doctoral research and I have hit a roadblock. Using my laptop and remote computing, some progress was possible in the last 10 to 15 days. But, I have to admit that this has been a difficult situation for me to focus on my research. Meanwhile, the outbreak, though saddening, is intriguing for a researcher. Tons of data on the outbreak is pouring in from all over the world everyday. So, I have decided to practice some data visualization technqiues using the data. I will be using python language and the bokeh library, in particular, to visualize and then embed the results here. The dataset I will be working on is that the COVID19 outbreak data for my home state of Tamil Nadu. The source is the official website of the Tamil Nadu health department dedicated for addressing the COVID19 outbreak. Hopefully, the website is regulary updated so that I can also regularly update the visualizations.
</p>

  <head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="3a840143-4bbb-4bd7-96a2-e22c8bc432c6" data-root-id="1075"></div>
            
          
        
      
      
        <script type="application/json" id="1268">
          {"60fdccd7-eb72-4f68-9e87-4e3737032f79":{"roots":{"references":[{"attributes":{"axis":{"id":"1015"},"dimension":1,"ticker":null},"id":"1018","type":"Grid"},{"attributes":{"overlay":{"id":"1025"}},"id":"1021","type":"BoxZoomTool"},{"attributes":{},"id":"1024","type":"HelpTool"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"blue"},"line_alpha":{"value":0.1},"line_color":{"value":"blue"},"top":{"field":"top"},"width":{"value":0.85},"x":{"field":"x"}},"id":"1072","type":"VBar"},{"attributes":{},"id":"1019","type":"PanTool"},{"attributes":{"data_source":{"id":"1070"},"glyph":{"id":"1071"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1072"},"selection_glyph":null,"view":{"id":"1074"}},"id":"1073","type":"GlyphRenderer"},{"attributes":{},"id":"1020","type":"WheelZoomTool"},{"attributes":{},"id":"1022","type":"SaveTool"},{"attributes":{},"id":"1023","type":"ResetTool"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1062","type":"BoxAnnotation"},{"attributes":{},"id":"1087","type":"UnionRenderers"},{"attributes":{},"id":"1088","type":"Selection"},{"attributes":{},"id":"1078","type":"CategoricalTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1025","type":"BoxAnnotation"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1056"},{"id":"1057"},{"id":"1058"},{"id":"1059"},{"id":"1060"},{"id":"1061"}]},"id":"1063","type":"Toolbar"},{"attributes":{},"id":"1090","type":"UnionRenderers"},{"attributes":{},"id":"1080","type":"BasicTickFormatter"},{"attributes":{},"id":"1091","type":"Selection"},{"attributes":{"source":{"id":"1070"}},"id":"1074","type":"CDSView"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1019"},{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"}]},"id":"1026","type":"Toolbar"},{"attributes":{"overlay":{"id":"1062"}},"id":"1058","type":"BoxZoomTool"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1082"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1050"}},"id":"1049","type":"CategoricalAxis"},{"attributes":{"source":{"id":"1033"}},"id":"1037","type":"CDSView"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"red"},"line_alpha":{"value":0.1},"line_color":{"value":"red"},"top":{"field":"top"},"width":{"value":0.85},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{"data_source":{"id":"1033"},"glyph":{"id":"1034"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1035"},"selection_glyph":null,"view":{"id":"1037"}},"id":"1036","type":"GlyphRenderer"},{"attributes":{"below":[{"id":"1049"}],"center":[{"id":"1051"},{"id":"1055"}],"left":[{"id":"1052"}],"plot_height":400,"renderers":[{"id":"1073"}],"title":{"id":"1039"},"toolbar":{"id":"1063"},"x_range":{"id":"1041"},"x_scale":{"id":"1045"},"y_range":{"id":"1043"},"y_scale":{"id":"1047"}},"id":"1038","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1060","type":"ResetTool"},{"attributes":{"fill_color":{"value":"blue"},"line_color":{"value":"blue"},"top":{"field":"top"},"width":{"value":0.85},"x":{"field":"x"}},"id":"1071","type":"VBar"},{"attributes":{"below":[{"id":"1012"}],"center":[{"id":"1014"},{"id":"1018"}],"left":[{"id":"1015"}],"plot_height":400,"renderers":[{"id":"1036"}],"title":{"id":"1002"},"toolbar":{"id":"1026"},"x_range":{"id":"1004"},"x_scale":{"id":"1008"},"y_range":{"id":"1006"},"y_scale":{"id":"1010"}},"id":"1001","subtype":"Figure","type":"Plot"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"id":"1041","type":"FactorRange"},{"attributes":{"data":{"top":[0,0,1,0,0,0,0,0,0,0,0,0,0,1,1,0,3,1,2,6,8,6,9,4,8,17,57,110,75,102],"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"selected":{"id":"1091"},"selection_policy":{"id":"1090"}},"id":"1070","type":"ColumnDataSource"},{"attributes":{"fill_color":{"value":"red"},"line_color":{"value":"red"},"top":{"field":"top"},"width":{"value":0.85},"x":{"field":"x"}},"id":"1034","type":"VBar"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"20pt"}},"id":"1039","type":"Title"},{"attributes":{},"id":"1050","type":"CategoricalTicker"},{"attributes":{},"id":"1082","type":"CategoricalTickFormatter"},{"attributes":{"end":130},"id":"1043","type":"Range1d"},{"attributes":{"children":[{"id":"1001"},{"id":"1038"}]},"id":"1075","type":"Column"},{"attributes":{},"id":"1056","type":"PanTool"},{"attributes":{},"id":"1045","type":"CategoricalScale"},{"attributes":{},"id":"1084","type":"BasicTickFormatter"},{"attributes":{},"id":"1047","type":"LinearScale"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"id":"1004","type":"FactorRange"},{"attributes":{"axis":{"id":"1049"},"ticker":null},"id":"1051","type":"Grid"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1084"},"major_label_text_font_size":"10pt","ticker":{"id":"1053"}},"id":"1052","type":"LinearAxis"},{"attributes":{"end":431},"id":"1006","type":"Range1d"},{"attributes":{},"id":"1053","type":"BasicTicker"},{"attributes":{},"id":"1008","type":"CategoricalScale"},{"attributes":{"axis":{"id":"1052"},"dimension":1,"ticker":null},"id":"1055","type":"Grid"},{"attributes":{},"id":"1013","type":"CategoricalTicker"},{"attributes":{"text":"Number of positive cases (Cumulative))","text_font_size":{"value":"20pt"}},"id":"1002","type":"Title"},{"attributes":{"data":{"top":[0,0,1,0,1,1,1,1,1,1,1,1,1,2,3,3,6,7,9,15,23,29,38,42,50,67,124,234,309,411],"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"selected":{"id":"1088"},"selection_policy":{"id":"1087"}},"id":"1033","type":"ColumnDataSource"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1080"},"major_label_text_font_size":"10pt","ticker":{"id":"1016"}},"id":"1015","type":"LinearAxis"},{"attributes":{},"id":"1057","type":"WheelZoomTool"},{"attributes":{},"id":"1061","type":"HelpTool"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1078"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1013"}},"id":"1012","type":"CategoricalAxis"},{"attributes":{},"id":"1059","type":"SaveTool"},{"attributes":{},"id":"1010","type":"LinearScale"},{"attributes":{"axis":{"id":"1012"},"ticker":null},"id":"1014","type":"Grid"},{"attributes":{},"id":"1016","type":"BasicTicker"}],"root_ids":["1075"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1268').textContent;
                  var render_items = [{"docid":"60fdccd7-eb72-4f68-9e87-4e3737032f79","root_ids":["1075"],"roots":{"1075":"3a840143-4bbb-4bd7-96a2-e22c8bc432c6"}}];
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
