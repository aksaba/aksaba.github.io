---
layout: post
title:  "Tracking the COVID19 Outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<div style="text-align:justify">
<p>
This is day 10 of the lock down which is in effect because of the worldwide COVID19 outbreak. I'm in the last stretch of my doctoral research and I have hit a roadblock. Using my laptop and remote computing, some progress was possible in the last 10 to 15 days. But, I have to admit that this has been a difficult situation for me to focus on my research. Meanwhile, the outbreak, though saddening, is intriguing phenomenon for any researcher. Tons of data on the outbreak is pouring in from all over the world everyday. So, I have decided to practice some data visualization technqiues making use of the data. I will be using python language (v3.8.2) and the <a href= "https://bokeh.org/" >Bokeh library </a>, in particular, to visualize and then embed the results here. The dataset I will be working on is the COVID19 outbreak data for my home state of Tamil Nadu. The source is the <a href="https://stopcorona.tn.gov.in/">official website</a> of the Tamil Nadu health department dedicated for addressing the COVID19 outbreak. Hopefully, the source is regulary updated so that I can also regularly update the visualizations.
</p>

<p>
Below presented are the cumulative and daily new positive cases of COVID19 in Tamil Nadu. 
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
    
      
        
          
          
            
              <div class="bk-root" id="df1d88d7-adc5-493b-bf2d-7b7bde1f5080" data-root-id="1080"></div>
            
          
        
      
      
        <script type="application/json" id="1251">
          {"cad3599c-59df-498b-85ed-b795900c6496":{"roots":{"references":[{"attributes":{},"id":"1062","type":"SaveTool"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1065","type":"BoxAnnotation"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{},"id":"1087","type":"BasicTickFormatter"},{"attributes":{},"id":"1089","type":"CategoricalTickFormatter"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1050","type":"LinearScale"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{},"id":"1064","type":"HelpTool"},{"attributes":{"overlay":{"id":"1065"}},"id":"1061","type":"BoxZoomTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1059"},{"id":"1060"},{"id":"1061"},{"id":"1062"},{"id":"1063"},{"id":"1064"},{"id":"1078"}]},"id":"1066","type":"Toolbar"},{"attributes":{},"id":"1063","type":"ResetTool"},{"attributes":{},"id":"1060","type":"WheelZoomTool"},{"attributes":{},"id":"1091","type":"Selection"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1089"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1053"}},"id":"1052","type":"CategoricalAxis"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1074"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1075"},"selection_glyph":null,"view":{"id":"1077"}},"id":"1076","type":"GlyphRenderer"},{"attributes":{},"id":"1092","type":"UnionRenderers"},{"attributes":{},"id":"1056","type":"BasicTicker"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1087"},"major_label_text_font_size":"10pt","ticker":{"id":"1056"}},"id":"1055","type":"LinearAxis"},{"attributes":{"axis":{"id":"1055"},"dimension":1,"ticker":null},"id":"1058","type":"Grid"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1075","type":"VBar"},{"attributes":{"source":{"id":"1001"}},"id":"1077","type":"CDSView"},{"attributes":{"children":[{"id":"1003"},{"id":"1042"}]},"id":"1080","type":"Column"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1039"}]},"id":"1027","type":"Toolbar"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"20pt"}},"id":"1043","type":"Title"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"source":{"id":"1001"}},"id":"1038","type":"CDSView"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"id":"1041","type":"FactorRange"},{"attributes":{},"id":"1083","type":"BasicTickFormatter"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1074","type":"VBar"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1078","type":"HoverTool"},{"attributes":{},"id":"1085","type":"CategoricalTickFormatter"},{"attributes":{"below":[{"id":"1052"}],"center":[{"id":"1054"},{"id":"1058"}],"left":[{"id":"1055"}],"plot_height":400,"renderers":[{"id":"1076"}],"title":{"id":"1043"},"toolbar":{"id":"1066"},"x_range":{"id":"1041"},"x_scale":{"id":"1048"},"y_range":{"id":"1046"},"y_scale":{"id":"1050"}},"id":"1042","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1059","type":"PanTool"},{"attributes":{},"id":"1048","type":"CategoricalScale"},{"attributes":{},"id":"1053","type":"CategoricalTicker"},{"attributes":{"axis":{"id":"1052"},"ticker":null},"id":"1054","type":"Grid"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@pos_counts"]]},"id":"1039","type":"HoverTool"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"id":"1002","type":"FactorRange"},{"attributes":{"data":{"daily_counts":["0","0","1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102"],"pos_counts":["0","0","1","0","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411"],"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"selected":{"id":"1091"},"selection_policy":{"id":"1092"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{"text":"Number of positive cases (Cumulative))","text_font_size":{"value":"20pt"}},"id":"1004","type":"Title"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"}],"left":[{"id":"1016"}],"plot_height":400,"renderers":[{"id":"1037"}],"title":{"id":"1004"},"toolbar":{"id":"1027"},"x_range":{"id":"1002"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1046","type":"DataRange1d"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1083"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{},"id":"1007","type":"DataRange1d"},{"attributes":{},"id":"1014","type":"CategoricalTicker"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1085"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1014"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1017","type":"BasicTicker"}],"root_ids":["1080"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1251').textContent;
                  var render_items = [{"docid":"cad3599c-59df-498b-85ed-b795900c6496","root_ids":["1080"],"roots":{"1080":"df1d88d7-adc5-493b-bf2d-7b7bde1f5080"}}];
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
