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
</div>
  <div class="bk-root" id="20dd8419-28c1-4214-b589-c25ed9d1da4d" data-root-id="1001"></div>
<head>
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
</head>
<script type="application/json" id="1134">
{"44075f9b-d1b0-4693-9fd1-e1b4bafc2d92":{"roots":{"references":[{"attributes":{"data_source":{"id":"1033"},"glyph":{"id":"1034"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1035"},"selection_glyph":null,"view":{"id":"1037"}},"id":"1036","type":"GlyphRenderer"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1019"},{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"}]},"id":"1026","type":"Toolbar"},{"attributes":{},"id":"1041","type":"CategoricalTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1025","type":"BoxAnnotation"},{"attributes":{"fill_color":{"value":"black"},"top":{"field":"top"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1034","type":"VBar"},{"attributes":{"formatter":{"id":"1041"},"major_label_orientation":1.5707963267948966,"ticker":{"id":"1013"}},"id":"1012","type":"CategoricalAxis"},{"attributes":{},"id":"1039","type":"BasicTickFormatter"},{"attributes":{"text":"Number of positive cases over time"},"id":"1002","type":"Title"},{"attributes":{},"id":"1008","type":"CategoricalScale"},{"attributes":{},"id":"1013","type":"CategoricalTicker"},{"attributes":{"end":431},"id":"1006","type":"Range1d"},{"attributes":{},"id":"1010","type":"LinearScale"},{"attributes":{"axis":{"id":"1012"},"ticker":null},"id":"1014","type":"Grid"},{"attributes":{"formatter":{"id":"1039"},"ticker":{"id":"1016"}},"id":"1015","type":"LinearAxis"},{"attributes":{"below":[{"id":"1012"}],"center":[{"id":"1014"},{"id":"1018"}],"left":[{"id":"1015"}],"plot_height":500,"plot_width":800,"renderers":[{"id":"1036"}],"title":{"id":"1002"},"toolbar":{"id":"1026"},"x_range":{"id":"1004"},"x_scale":{"id":"1008"},"y_range":{"id":"1006"},"y_scale":{"id":"1010"}},"id":"1001","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1016","type":"BasicTicker"},{"attributes":{"axis":{"id":"1015"},"dimension":1,"ticker":null},"id":"1018","type":"Grid"},{"attributes":{"overlay":{"id":"1025"}},"id":"1021","type":"BoxZoomTool"},{"attributes":{},"id":"1024","type":"HelpTool"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"id":"1004","type":"FactorRange"},{"attributes":{"data":{"top":[0,0,1,0,1,1,1,1,1,1,1,1,1,2,3,3,6,7,9,15,23,29,38,42,50,67,124,234,309,411],"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr"]},"selected":{"id":"1044"},"selection_policy":{"id":"1043"}},"id":"1033","type":"ColumnDataSource"},{"attributes":{},"id":"1019","type":"PanTool"},{"attributes":{},"id":"1020","type":"WheelZoomTool"},{"attributes":{},"id":"1043","type":"UnionRenderers"},{"attributes":{},"id":"1044","type":"Selection"},{"attributes":{},"id":"1022","type":"SaveTool"},{"attributes":{},"id":"1023","type":"ResetTool"},{"attributes":{"source":{"id":"1033"}},"id":"1037","type":"CDSView"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"black"},"line_alpha":{"value":0.1},"top":{"field":"top"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1035","type":"VBar"}],"root_ids":["1001"]},"title":"Bokeh Application","version":"2.0.1"}}
</script>
<script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1134').textContent;
                  var render_items = [{"docid":"44075f9b-d1b0-4693-9fd1-e1b4bafc2d92","root_ids":["1001"],"roots":{"1001":"20dd8419-28c1-4214-b589-c25ed9d1da4d"}}];
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


