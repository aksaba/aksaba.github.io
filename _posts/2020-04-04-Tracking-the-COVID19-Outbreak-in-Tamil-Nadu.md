---
layout: post
title:  "Tracking the COVID19 Outbreak in Tamil Nadu"
date:   2020-04-04 09:50:00 +0530
categories: jekyll update


---

<p>Graph updated: 2230 hours 19 April 2020 </p>
<head>
    
      <meta charset="utf-8">
      <title>Bokeh Plot</title>
      
      
        
          
        
        
          
        <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
        <script type="text/javascript">
            Bokeh.set_log_level("info");
        </script>
        
      
      
    
  </head>
  
  
  <body>
    
      
        
          
          
            
              <div class="bk-root" id="50d3f370-e36a-426d-97a1-456f36be2bc8" data-root-id="1080"></div>
            
          
        
      
      
        <script type="application/json" id="1251">
          {"d66d3790-77e1-43ab-871f-db27f219bb8e":{"roots":{"references":[{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{"axis":{"id":"1052"},"ticker":null},"id":"1054","type":"Grid"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1059","type":"PanTool"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{},"id":"1088","type":"CategoricalTickFormatter"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{},"id":"1056","type":"BasicTicker"},{"attributes":{},"id":"1090","type":"BasicTickFormatter"},{"attributes":{},"id":"1050","type":"LinearScale"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1090"},"major_label_text_font_size":"10pt","ticker":{"id":"1056"}},"id":"1055","type":"LinearAxis"},{"attributes":{"axis":{"id":"1055"},"dimension":1,"ticker":null},"id":"1058","type":"Grid"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1059"},{"id":"1060"},{"id":"1061"},{"id":"1062"},{"id":"1063"},{"id":"1064"},{"id":"1078"}]},"id":"1066","type":"Toolbar"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1074"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1075"},"selection_glyph":null,"view":{"id":"1077"}},"id":"1076","type":"GlyphRenderer"},{"attributes":{},"id":"1053","type":"CategoricalTicker"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1088"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1053"}},"id":"1052","type":"CategoricalAxis"},{"attributes":{},"id":"1091","type":"UnionRenderers"},{"attributes":{},"id":"1046","type":"DataRange1d"},{"attributes":{},"id":"1048","type":"CategoricalScale"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1075","type":"VBar"},{"attributes":{},"id":"1092","type":"Selection"},{"attributes":{"source":{"id":"1001"}},"id":"1077","type":"CDSView"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"children":[{"id":"1003"},{"id":"1041"}]},"id":"1080","type":"Column"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1039"}]},"id":"1027","type":"Toolbar"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"overlay":{"id":"1065"}},"id":"1061","type":"BoxZoomTool"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"below":[{"id":"1052"}],"center":[{"id":"1054"},{"id":"1058"}],"left":[{"id":"1055"}],"plot_height":400,"renderers":[{"id":"1076"}],"title":{"id":"1042"},"toolbar":{"id":"1066"},"x_range":{"id":"1044"},"x_scale":{"id":"1048"},"y_range":{"id":"1046"},"y_scale":{"id":"1050"}},"id":"1041","subtype":"Figure","type":"Plot"},{"attributes":{"source":{"id":"1001"}},"id":"1038","type":"CDSView"},{"attributes":{},"id":"1064","type":"HelpTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1078","type":"HoverTool"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1074","type":"VBar"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"20pt"}},"id":"1042","type":"Title"},{"attributes":{},"id":"1060","type":"WheelZoomTool"},{"attributes":{},"id":"1062","type":"SaveTool"},{"attributes":{},"id":"1063","type":"ResetTool"},{"attributes":{},"id":"1084","type":"CategoricalTickFormatter"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@pos_counts"]]},"id":"1039","type":"HoverTool"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"]},"id":"1002","type":"FactorRange"},{"attributes":{"data":{"daily_counts":["0","0","1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105"],"pos_counts":["0","0","1","0","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477"],"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"]},"selected":{"id":"1092"},"selection_policy":{"id":"1091"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{},"id":"1086","type":"BasicTickFormatter"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{"text":"Number of positive cases (Cumulative)","text_font_size":{"value":"20pt"}},"id":"1004","type":"Title"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"}],"left":[{"id":"1016"}],"plot_height":400,"plot_width":800,"renderers":[{"id":"1037"}],"title":{"id":"1004"},"toolbar":{"id":"1027"},"x_range":{"id":"1002"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"]},"id":"1044","type":"FactorRange"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{},"id":"1014","type":"CategoricalTicker"},{"attributes":{},"id":"1007","type":"DataRange1d"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1086"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1084"},"major_label_orientation":1.5707963267948966,"ticker":{"id":"1014"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1065","type":"BoxAnnotation"}],"root_ids":["1080"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1251').textContent;
                  var render_items = [{"docid":"d66d3790-77e1-43ab-871f-db27f219bb8e","root_ids":["1080"],"roots":{"1080":"50d3f370-e36a-426d-97a1-456f36be2bc8"}}];
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
    
      
        
          
          
            
              <div class="bk-root" id="f4eb3fd4-4cc8-4c98-b963-ba0409f2872f" data-root-id="1001"></div>
            
          
        
      
      
        <script type="application/json" id="1268">
          {"6f54113b-be81-4d22-af8b-7861b2e8ccfe":{"roots":{"references":[{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"white"},"line_alpha":{"value":0.1},"line_color":{"value":"green"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1049","type":"Circle"},{"attributes":{"data_source":{"id":"1054"},"glyph":{"id":"1055"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1056"},"selection_glyph":null,"view":{"id":"1058"},"y_range_name":"foo"},"id":"1057","type":"GlyphRenderer"},{"attributes":{"overlay":{"id":"1025"}},"id":"1021","type":"BoxZoomTool"},{"attributes":{},"id":"1022","type":"SaveTool"},{"attributes":{"data":{"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"],"y":["nan","nan","nan","nan","63","74","75","76","77","79","88","98","140","291","320","333","412","443","552","743","890","1039","1243","1500","1763","2040","2354","2726","3272","3684","4248","4612","5061","5305","6095","7267","8410","9842","10655","12746","19255","21994","26005","29673","35036","40876"]},"selected":{"id":"1067"},"selection_policy":{"id":"1068"}},"id":"1047","type":"ColumnDataSource"},{"attributes":{},"id":"1019","type":"PanTool"},{"attributes":{},"id":"1020","type":"WheelZoomTool"},{"attributes":{"fill_color":{"value":"white"},"line_color":{"value":"green"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1048","type":"Circle"},{"attributes":{"data_source":{"id":"1047"},"glyph":{"id":"1048"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1049"},"selection_glyph":null,"view":{"id":"1051"}},"id":"1050","type":"GlyphRenderer"},{"attributes":{},"id":"1024","type":"HelpTool"},{"attributes":{},"id":"1023","type":"ResetTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@y"]]},"id":"1052","type":"HoverTool"},{"attributes":{"source":{"id":"1047"}},"id":"1051","type":"CDSView"},{"attributes":{"data":{"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"],"y":["nan","nan","nan","nan","1.59","1.35","1.33","1.32","1.3","1.27","1.14","1.02","0.71","0.69","0.94","0.9","1.46","1.58","1.63","2.02","2.58","2.79","3.06","2.8","2.84","3.28","5.27","8.58","9.44","11.16","11.42","12.38","12.27","13.01","12.11","11.48","10.83","9.85","10.09","9.2","6.25","5.65","4.87","4.46","3.92","3.61"]},"selected":{"id":"1088"},"selection_policy":{"id":"1089"}},"id":"1054","type":"ColumnDataSource"},{"attributes":{},"id":"1088","type":"Selection"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1055","type":"Line"},{"attributes":{},"id":"1089","type":"UnionRenderers"},{"attributes":{},"id":"1040","type":"CategoricalTickFormatter"},{"attributes":{"source":{"id":"1054"}},"id":"1058","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1056","type":"Line"},{"attributes":{"label":{"value":"%positive cases"},"renderers":[{"id":"1057"}]},"id":"1069","type":"LegendItem"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1079"},"major_label_text_font_size":"10pt","ticker":{"id":"1080"},"y_range_name":"foo"},"id":"1075","type":"LinearAxis"},{"attributes":{},"id":"1090","type":"Selection"},{"attributes":{},"id":"1091","type":"UnionRenderers"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1025","type":"BoxAnnotation"},{"attributes":{},"id":"1065","type":"Selection"},{"attributes":{},"id":"1066","type":"UnionRenderers"},{"attributes":{},"id":"1067","type":"Selection"},{"attributes":{},"id":"1068","type":"UnionRenderers"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1019"},{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1052"}]},"id":"1026","type":"Toolbar"},{"attributes":{"source":{"id":"1034"}},"id":"1038","type":"CDSView"},{"attributes":{"items":[{"id":"1046"},{"id":"1069"}],"location":"top_left"},"id":"1045","type":"Legend"},{"attributes":{"line_alpha":0.75,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1035","type":"Line"},{"attributes":{"line_alpha":0.1,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1036","type":"Line"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"white"},"line_alpha":{"value":0.1},"line_color":{"value":"red"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1072","type":"Circle"},{"attributes":{"data":{"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"],"y":["nan","nan","nan","nan","1.59","1.35","1.33","1.32","1.3","1.27","1.14","1.02","0.71","0.69","0.94","0.9","1.46","1.58","1.63","2.02","2.58","2.79","3.06","2.8","2.84","3.28","5.27","8.58","9.44","11.16","11.42","12.38","12.27","13.01","12.11","11.48","10.83","9.85","10.09","9.2","6.25","5.65","4.87","4.46","3.92","3.61"]},"selected":{"id":"1090"},"selection_policy":{"id":"1091"}},"id":"1070","type":"ColumnDataSource"},{"attributes":{"fill_color":{"value":"white"},"line_color":{"value":"red"},"size":{"units":"screen","value":8},"x":{"field":"x"},"y":{"field":"y"}},"id":"1071","type":"Circle"},{"attributes":{"data_source":{"id":"1070"},"glyph":{"id":"1071"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1072"},"selection_glyph":null,"view":{"id":"1074"},"y_range_name":"foo"},"id":"1073","type":"GlyphRenderer"},{"attributes":{"source":{"id":"1070"}},"id":"1074","type":"CDSView"},{"attributes":{},"id":"1042","type":"BasicTickFormatter"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1040"},"major_label_orientation":1.5707963267948966,"ticker":{"id":"1013"}},"id":"1012","type":"CategoricalAxis"},{"attributes":{"below":[{"id":"1012"}],"center":[{"id":"1014"},{"id":"1018"},{"id":"1045"}],"extra_y_ranges":{"foo":{"id":"1033"}},"left":[{"id":"1015"}],"plot_height":400,"plot_width":800,"renderers":[{"id":"1037"},{"id":"1050"},{"id":"1057"},{"id":"1073"}],"right":[{"id":"1075"}],"title":{"id":"1002"},"toolbar":{"id":"1026"},"x_range":{"id":"1004"},"x_scale":{"id":"1008"},"y_range":{"id":"1006"},"y_scale":{"id":"1010"}},"id":"1001","subtype":"Figure","type":"Plot"},{"attributes":{"data_source":{"id":"1034"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"end":15},"id":"1033","type":"Range1d"},{"attributes":{"text":"Samples collected and percentage of positive samples","text_font_size":{"value":"15pt"}},"id":"1002","type":"Title"},{"attributes":{"factors":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"]},"id":"1004","type":"FactorRange"},{"attributes":{},"id":"1079","type":"BasicTickFormatter"},{"attributes":{"data":{"x":["05-Mar","06-Mar","07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr"],"y":["nan","nan","nan","nan","63","74","75","76","77","79","88","98","140","291","320","333","412","443","552","743","890","1039","1243","1500","1763","2040","2354","2726","3272","3684","4248","4612","5061","5305","6095","7267","8410","9842","10655","12746","19255","21994","26005","29673","35036","40876"]},"selected":{"id":"1065"},"selection_policy":{"id":"1066"}},"id":"1034","type":"ColumnDataSource"},{"attributes":{},"id":"1008","type":"CategoricalScale"},{"attributes":{},"id":"1080","type":"BasicTicker"},{"attributes":{},"id":"1013","type":"CategoricalTicker"},{"attributes":{"end":50000},"id":"1006","type":"Range1d"},{"attributes":{},"id":"1010","type":"LinearScale"},{"attributes":{"axis":{"id":"1012"},"ticker":null},"id":"1014","type":"Grid"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1042"},"major_label_text_font_size":"10pt","ticker":{"id":"1016"}},"id":"1015","type":"LinearAxis"},{"attributes":{},"id":"1016","type":"BasicTicker"},{"attributes":{"axis":{"id":"1015"},"dimension":1,"ticker":null,"visible":false},"id":"1018","type":"Grid"},{"attributes":{"label":{"value":"samples collected"},"renderers":[{"id":"1037"}]},"id":"1046","type":"LegendItem"}],"root_ids":["1001"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1268').textContent;
                  var render_items = [{"docid":"6f54113b-be81-4d22-af8b-7861b2e8ccfe","root_ids":["1001"],"roots":{"1001":"f4eb3fd4-4cc8-4c98-b963-ba0409f2872f"}}];
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
P. S.
Apart from the official Python and Bokeh documentations and numerous google searches to check and correct minor issues in the python code, there are a few sources which helped me a lot in writing this code. I'm listing them below:
<ul>
<li>   <a href="https://stackoverflow.com/questions/49722791/python-bokeh-vbar-hover-tool"> Stackoverflow question on adding hovertool to bargraph </a> </li>

<li> <a href="https://stackoverflow.com/questions/25050311/extract-first-item-of-each-sublist"> Stack Overflow question on list comprehension </a></li>

<li> Stack Overflow questions <a href="https://stackoverflow.com/questions/25199665/one-chart-with-two-different-y-axis-ranges-in-bokeh/30914348#30914348">(1) </a><a href = "https://stackoverflow.com/questions/29267141/bokeh-add-label-to-second-axis-on-the-right">(2)</a> on adding second axis.</li>
</ul>
</p>



