---
layout: default
---



## Codes

### **Enhancing English Writing Using a Local Language Model: A Step-by-Step Guide**

Writing fluently in English can be challenging for non-native speakers. Even with a solid grasp of vocabulary and grammar, nuances in tone, style, and sentence structure can be difficult to capture. For those who work regularly in English but want to enhance fluency and clarity in their writing, language models (LMs) can provide valuable assistance.

However, many of the most powerful LMs require a subscription or have strict data-sharing limitations, which may not be suitable for everyone. This is where open-source, locally run models can be a fantastic alternative.

### **Why Choose a Local Language Model?**

Using a local LM over a commercial, cloud-based model has several advantages:

* **Cost-Effective**: Local models are often open-source and free to use, bypassing subscription fees.
* **Privacy and Security**: Running an LM locally keeps data off third-party servers, ideal for sensitive or confidential work.
* **Customization**: Local models can often be fine-tuned for specific tasks, tailoring them to your unique needs.

One promising option in this space is Microsoft’s Phi family of LMs, which are designed to support a range of tasks, including text editing and enhancement. In this guide, we’ll walk you through the steps for setting up and using a Phi LM locally to edit and improve sentences.

---

### **Step 1: Setting Up the Prerequisites**

To begin, ensure you have the following prerequisites:

* **Python**: Make sure Python (version 3.7 or newer) is installed on your machine. You can download it from [Python’s official site](https://www.python.org/downloads/).
    
* **Python Libraries**: Some libraries are required to interact with and run the LM. Run the following command in your terminal or command prompt to install the necessary packages:
    
    bash
    
    Copy code
    
    `pip install transformers torch sentencepiece` 
    
* **Download the Language Model**: You’ll need to download the Phi LM  from a repository that supports its use, such as the [Hugging Face model hub](https://huggingface.co/microsoft/Phi-3-mini-4k-instruct-gguf). This can be done programmatically within the code itself.
    

---

### **Step 2: Loading and Initializing the Phi Language Model**

With the prerequisites in place, we can load and initialize the language model. Here’s a simplified breakdown of the process using the code provided:

1.  **Import the Required Libraries**:
    
    * The `transformers` library is essential for loading and interacting with LMs like Phi.
    
    python
    
    Copy code
    
    `from transformers import AutoModelForCausalLM, AutoTokenizer` 
    
2.  **Load the Model and Tokenizer**:
    
    * The `AutoModelForCausalLM` and `AutoTokenizer` classes load the model and tokenizer, respectively, which work together to process and interpret the input text.
    * Specify the model checkpoint path as shown below:
    
    python
    
    Copy code
    
    `model_name = "microsoft/phi"
    model = AutoModelForCausalLM.from_pretrained(model_name)
    tokenizer = AutoTokenizer.from_pretrained(model_name)` 
    
3.  **Move Model to GPU (Optional)**:
    
    * If you have a GPU available, moving the model to it can greatly speed up processing. The following line achieves this:
    
    python
    
    Copy code
    
    `model.to("cuda")  # Use "cpu" if GPU is not available` 
    

---

### **Step 3: Defining the Editing Function**

The core of this code involves an editing function that takes in text, processes it using the model, and outputs a more fluent version. This function typically follows these steps:

1.  **Tokenize the Input Text**:
    
    * Convert the input text into a format the model can process. Tokenization is necessary to break down the text into smaller pieces.
    
    python
    
    Copy code
    
    `inputs = tokenizer(input_text, return_tensors="pt").to("cuda")` 
    
2.  **Generate Output**:
    
    * Use the model to generate a response based on the input. Adjust parameters like `max_length` and `temperature` to control the response length and creativity, respectively.
    
    python
    
    Copy code
    
    `output = model.generate(
        **inputs,
        max_length=100,
        num_return_sequences=1,
        temperature=0.8
    )` 
    
3.  **Decode the Output**:
    
    * Convert the generated tokens back into readable text. This is done with the tokenizer’s decode function, ensuring the output text is clean.
    
    python
    
    Copy code
    
    `edited_text = tokenizer.decode(output[0], skip_special_tokens=True)` 
    

---

### **Step 4: Running the Model to Edit Sentences**

With everything set up, you can now use the model to edit sentences! Here’s how you can do it:

1.  **Input Your Sentence**:
    
    * Call the editing function, passing in the text you’d like to improve.
    
    python
    
    Copy code
    
    `input_text = "This are example sentence needing improvement."
    edited_text = edit_text(input_text)
    print("Edited Text:", edited_text)` 
    
2.  **Review and Iterate**:
    
    * Since language models may produce varied results, it can be helpful to adjust parameters like temperature or max length based on the text type and desired tone.



---

Using a local LM like Microsoft’s Phi model allows you to edit sentences without relying on cloud-based services, maintaining control over your data and avoiding subscription costs. With a few lines of code, you can create a reliable tool to help your writing sound fluent and natural. Try it out to see the difference it can make in your work!
### Tracking the COVID19 Outbreak in Tamil Nadu

Graphs updated: 2215 hours 03 June 2020 

<head>
<script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-2.0.1.min.js" integrity="sha384-JpP8FXbgAZLkfur7LiK3j9AGBhHNIvF742meBJrjO2ShJDhCG2I1uVvW+0DUtrmc" crossorigin="anonymous"></script>
<script type="text/javascript">
            Bokeh.set_log_level("info");
</script>
</head>
<body>
<div class="bk-root" id="d8a161ae-1ed5-43bf-87f5-e382d476e3f3" data-root-id="1086"></div>
 <script type="application/json" id="1233">
          {"966c7ea0-3f61-4320-98ee-e5e25b79a286":{"roots":{"references":[{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":1071},"id":"1044","type":"Label"},{"attributes":{},"id":"1050","type":"DataRange1d"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1089"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1092","type":"BasicTickFormatter"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1069","type":"BoxAnnotation"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{"text":"Number of daily positive cases","text_font_size":{"value":"15pt"}},"id":"1046","type":"Title"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"below":[{"id":"1056"}],"center":[{"id":"1058"},{"id":"1062"},{"id":"1044"}],"left":[{"id":"1059"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1080"}],"title":{"id":"1046"},"toolbar":{"id":"1070"},"x_range":{"id":"1048"},"x_scale":{"id":"1052"},"y_range":{"id":"1050"},"y_scale":{"id":"1054"}},"id":"1045","subtype":"Figure","type":"Plot"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@pos_counts"]]},"id":"1042","type":"HoverTool"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1094"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1082"}},"id":"1056","type":"CategoricalAxis"},{"attributes":{"interval":2},"id":"1082","type":"SingleIntervalTicker"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"id":"1048","type":"FactorRange"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1063"},{"id":"1064"},{"id":"1065"},{"id":"1066"},{"id":"1067"},{"id":"1068"},{"id":"1084"}]},"id":"1070","type":"Toolbar"},{"attributes":{},"id":"1063","type":"PanTool"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1078"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1079"},"selection_glyph":null,"view":{"id":"1081"}},"id":"1080","type":"GlyphRenderer"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1078","type":"VBar"},{"attributes":{"source":{"id":"1001"}},"id":"1039","type":"CDSView"},{"attributes":{},"id":"1096","type":"Selection"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"daily_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1079","type":"VBar"},{"attributes":{},"id":"1097","type":"UnionRenderers"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{"source":{"id":"1001"}},"id":"1081","type":"CDSView"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@daily_counts"]]},"id":"1084","type":"HoverTool"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1042"}]},"id":"1028","type":"Toolbar"},{"attributes":{"data":{"daily_counts":["1","0","0","0","0","0","0","0","0","0","0","1","1","0","3","1","2","6","8","6","9","4","8","17","57","110","75","102","74","86","50","69","48","96","77","58","106","98","31","38","25","56","49","105","43","76","33","54","72","66","64","52","121","104","161","203","231","266","527","508","771","580","600","526","669","798","716","509","447","434","477","639","536","688","743","776","786","759","765","805","646","817","827","874","938","1149","1162","1091"],"pos_counts":["1","1","1","1","1","1","1","1","1","1","1","2","3","3","6","7","9","15","23","29","38","42","50","67","124","234","309","411","485","571","621","690","738","834","911","969","1075","1173","1204","1242","1267","1323","1372","1477","1520","1596","1629","1683","1755","1821","1885","1937","2058","2162","2323","2526","2757","3023","3550","4058","4829","5409","6009","6535","7204","8002","8718","9227","9674","10108","10585","11224","11760","12448","13191","13967","14753","15512","16277","17082","17728","18545","19372","20246","21184","22333","23495","24586"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"selected":{"id":"1096"},"selection_policy":{"id":"1097"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"axis":{"id":"1056"},"ticker":null},"id":"1058","type":"Grid"},{"attributes":{},"id":"1089","type":"BasicTickFormatter"},{"attributes":{"children":[{"id":"1004"},{"id":"1045"}]},"id":"1086","type":"Column"},{"attributes":{},"id":"1052","type":"CategoricalScale"},{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1092"},"major_label_text_font_size":"10pt","ticker":{"id":"1060"}},"id":"1059","type":"LinearAxis"},{"attributes":{},"id":"1054","type":"LinearScale"},{"attributes":{},"id":"1060","type":"BasicTicker"},{"attributes":{"axis":{"id":"1059"},"dimension":1,"ticker":null},"id":"1062","type":"Grid"},{"attributes":{},"id":"1091","type":"CategoricalTickFormatter"},{"attributes":{},"id":"1064","type":"WheelZoomTool"},{"attributes":{},"id":"1068","type":"HelpTool"},{"attributes":{"overlay":{"id":"1069"}},"id":"1065","type":"BoxZoomTool"},{"attributes":{},"id":"1066","type":"SaveTool"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":23986},"id":"1002","type":"Label"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1002"}],"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"}],"title":{"id":"1005"},"toolbar":{"id":"1028"},"x_range":{"id":"1003"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1004","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1067","type":"ResetTool"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"id":"1003","type":"FactorRange"},{"attributes":{"text":"Number of positive cases (Cumulative)","text_font_size":{"value":"15pt"}},"id":"1005","type":"Title"},{"attributes":{},"id":"1094","type":"CategoricalTickFormatter"},{"attributes":{"interval":2},"id":"1040","type":"SingleIntervalTicker"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1091"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1040"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"pos_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{},"id":"1012","type":"LinearScale"},{"attributes":{},"id":"1008","type":"DataRange1d"}],"root_ids":["1086"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1233').textContent;
                  var render_items = [{"docid":"966c7ea0-3f61-4320-98ee-e5e25b79a286","root_ids":["1086"],"roots":{"1086":"d8a161ae-1ed5-43bf-87f5-e382d476e3f3"}}];
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
 <div class="bk-root" id="af405316-c655-4b89-8170-d6ded7c958b8" data-root-id="1002"></div>
  <script type="application/json" id="1239">
          {"a20949d5-e5ca-4ed5-b8c5-f89b50ec8a4f":{"roots":{"references":[{"attributes":{"axis_label":"No. of Samples (in thousands)","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1042"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"label":{"value":"Processed samples"},"renderers":[{"id":"1038"}]},"id":"1047","type":"LegendItem"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null,"visible":false},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","1.28","0.98","1.74","1.95","1.76","2.41","2.95","3.01","3.18","2.93","2.97","3.49","5.27","8.58","10.77","12.84","12.63","13.36","13.16","13.52","13.11","12.53","11.76","11.08","11.38","10.1","8.34","7.55","6.33","5.76","4.8","4.43","3.84","3.53","3.19","2.88","2.73","2.56","2.39","2.28","2.25","2.18","2.13","2.14","2.14","2.17","2.33","2.46","2.72","2.83","2.92","2.99","3.11","3.3","3.43","3.45","3.46","3.49","3.54","3.56","3.65","3.76","3.84","3.93","4.02","4.09","4.17","4.25","4.30","4.39","4.46","4.55","4.64","4.77","4.90","5.02"]},"selected":{"id":"1078"},"selection_policy":{"id":"1077"}},"id":"1050","type":"ColumnDataSource"},{"attributes":{"data_source":{"id":"1050"},"glyph":{"id":"1051"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1052"},"selection_glyph":null,"view":{"id":"1054"},"y_range_name":"foo"},"id":"1053","type":"GlyphRenderer"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["Value","@y"]]},"id":"1048","type":"HoverTool"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1051","type":"Line"},{"attributes":{"source":{"id":"1050"}},"id":"1054","type":"CDSView"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1052","type":"Line"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"label":{"value":"% total positive cases"},"renderers":[{"id":"1053"}]},"id":"1063","type":"LegendItem"},{"attributes":{},"id":"1094","type":"UnionRenderers"},{"attributes":{},"id":"1095","type":"Selection"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":450.215},"id":"1001","type":"Label"},{"attributes":{"line_alpha":0.1,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1037","type":"Line"},{"attributes":{"items":[{"id":"1047"},{"id":"1063"},{"id":"1079"}],"location":[1,140.21499999999997]},"id":"1046","type":"Legend"},{"attributes":{},"id":"1061","type":"UnionRenderers"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{},"id":"1062","type":"Selection"},{"attributes":{"line_alpha":0.75,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1065","type":"Line"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"],"y":["nan","nan","1.69","1.43","1.35","1.35","1.3","1.27","1.16","1.04","0.72","0.85","0.85","0.65","1.45","1.67","1.56","2.25","2.69","2.81","3.01","2.72","2.79","3.13","4.97","8.33","10.5","12.59","12.34","13.06","12.86","13.01","12.59","12","11.07","10.46","10.73","9.48","7.67","6.73","5.34","4.45","3.46","3.14","2.63","2.08","1.85","1.55","1.34","1.17","1.06","0.95","0.98","0.93","0.95","1","1.07","1.16","1.38","1.54","1.84","2","2.12","2.13","2.24","2.43","2.56","2.61","2.64","2.56","2.33","2.21","2.26","2.25","2.1","2.14","2.05","2.09","2.01","2.05","2.00","2.01","2.00","1.97","1.98","2.01","2.11","2.18"]},"selected":{"id":"1095"},"selection_policy":{"id":"1094"}},"id":"1064","type":"ColumnDataSource"},{"attributes":{"data_source":{"id":"1064"},"glyph":{"id":"1065"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1066"},"selection_glyph":null,"view":{"id":"1068"},"y_range_name":"foo"},"id":"1067","type":"GlyphRenderer"},{"attributes":{"source":{"id":"1064"}},"id":"1068","type":"CDSView"},{"attributes":{"line_alpha":0.1,"line_color":"blue","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1066","type":"Line"},{"attributes":{"label":{"value":"% active positive cases"},"renderers":[{"id":"1067"}]},"id":"1079","type":"LegendItem"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1048"}]},"id":"1027","type":"Toolbar"},{"attributes":{"source":{"id":"1035"}},"id":"1039","type":"CDSView"},{"attributes":{},"id":"1042","type":"BasicTickFormatter"},{"attributes":{},"id":"1077","type":"UnionRenderers"},{"attributes":{"line_alpha":0.75,"line_color":"green","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1036","type":"Line"},{"attributes":{},"id":"1078","type":"Selection"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"],"y":["nan","nan","0.059","0.07","0.074","0.074","0.077","0.079","0.086","0.096","0.139","0.234","0.235","0.306","0.345","0.359","0.512","0.623","0.78","0.962","1.195","1.435","1.682","1.92","2.354","2.726","2.868","3.2","3.841","4.273","4.72","5.104","5.631","6.658","7.749","8.748","9.448","11.61","14.438","16.452","20.01","22.951","28.564","33.33","39.602","45.178","51.135","58.519","64.351","71.211","79.018","84.958","91.281","99.14","109.054","118.098","129.097","139.152","152.627","164.751","177.601","191.378","205.495","218.847","231.692","242.617","254.335","267.768","279.266","289.955","298.645","315.026","321.973","331.465","343.227","355.226","367.436","379.199","390.604","402.074","411.801","422.368","434.06","444.558","456.667","468.593","479.61","490.215"]},"selected":{"id":"1062"},"selection_policy":{"id":"1061"}},"id":"1035","type":"ColumnDataSource"},{"attributes":{},"id":"1044","type":"CategoricalTickFormatter"},{"attributes":{"interval":2},"id":"1081","type":"SingleIntervalTicker"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1085"},"major_label_text_font_size":"10pt","ticker":{"id":"1084"},"y_range_name":"foo"},"id":"1080","type":"LinearAxis"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"},{"id":"1046"},{"id":"1001"}],"extra_y_ranges":{"foo":{"id":"1034"}},"left":[{"id":"1016"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1038"},{"id":"1053"},{"id":"1067"}],"right":[{"id":"1080"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{"text":"Samples processed and percentage of positive samples","text_font_size":{"value":"15pt"}},"id":"1003","type":"Title"},{"attributes":{"end":15},"id":"1034","type":"Range1d"},{"attributes":{"data_source":{"id":"1035"},"glyph":{"id":"1036"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1037"},"selection_glyph":null,"view":{"id":"1039"}},"id":"1038","type":"GlyphRenderer"},{"attributes":{},"id":"1084","type":"BasicTicker"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"id":"1005","type":"FactorRange"},{"attributes":{},"id":"1085","type":"BasicTickFormatter"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{"end":495.215},"id":"1007","type":"Range1d"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1044"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1081"}},"id":"1013","type":"CategoricalAxis"}],"root_ids":["1002"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1239').textContent;
                  var render_items = [{"docid":"a20949d5-e5ca-4ed5-b8c5-f89b50ec8a4f","root_ids":["1002"],"roots":{"1002":"af405316-c655-4b89-8170-d6ded7c958b8"}}];
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
  <div class="bk-root" id="4d66c5e5-d30b-45cf-9921-430aac3a3dea" data-root-id="1003"></div>
  <script type="application/json" id="1193">
          {"41fd2329-0e7a-453e-a6bc-bc40b3b2f7db":{"roots":{"references":[{"attributes":{"line_alpha":0.1,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1043","type":"Line"},{"attributes":{"axis":{"id":"1014"},"ticker":null},"id":"1016","type":"Grid"},{"attributes":{"axis_label":"Count","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1050"},"major_label_text_font_size":"10pt","ticker":{"id":"1018"}},"id":"1017","type":"LinearAxis"},{"attributes":{},"id":"1018","type":"BasicTicker"},{"attributes":{"axis":{"id":"1017"},"dimension":1,"ticker":null},"id":"1020","type":"Grid"},{"attributes":{"overlay":{"id":"1027"}},"id":"1023","type":"BoxZoomTool"},{"attributes":{},"id":"1026","type":"HelpTool"},{"attributes":{},"id":"1021","type":"PanTool"},{"attributes":{},"id":"1051","type":"UnionRenderers"},{"attributes":{},"id":"1022","type":"WheelZoomTool"},{"attributes":{},"id":"1052","type":"Selection"},{"attributes":{},"id":"1024","type":"SaveTool"},{"attributes":{},"id":"1025","type":"ResetTool"},{"attributes":{"line_alpha":0.75,"line_color":"red","line_width":3.5,"x":{"field":"x"},"y":{"field":"y"}},"id":"1042","type":"Line"},{"attributes":{"source":{"id":"1041"}},"id":"1045","type":"CDSView"},{"attributes":{"items":[{"id":"1055"}],"location":[1,212.0]},"id":"1054","type":"Legend"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1037"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1038"},"selection_glyph":null,"view":{"id":"1040"}},"id":"1039","type":"GlyphRenderer"},{"attributes":{"data":{"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"],"y":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","4.35","3.45","2.63","2.38","2","1.49","0.81","0.43","0.32","0.24","0.62","0.88","0.97","1.01","1.08","0.96","0.99","1.03","1.02","0.94","1","1.13","1.18","1.13","1.09","1.02","1.12","1.13","1.1","1.19","1.25","1.26","1.27","1.24","1.21","1.25","1.16","1.11","1.05","0.99","0.87","0.81","0.72","0.68","0.67","0.67","0.65","0.66","0.7","0.69","0.68","0.7","0.7","0.69","0.69","0.67","0.66","0.67","0.66","0.66","0.68","0.69","0.72","0.72","0.75","0.76","0.76","0.77","0.78","0.80"]},"selected":{"id":"1070"},"selection_policy":{"id":"1069"}},"id":"1041","type":"ColumnDataSource"},{"attributes":{"source":{"id":"1001"}},"id":"1040","type":"CDSView"},{"attributes":{"label":{"value":"% mortality rate"},"renderers":[{"id":"1044"}]},"id":"1055","type":"LegendItem"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1027","type":"BoxAnnotation"},{"attributes":{"interval":2},"id":"1057","type":"SingleIntervalTicker"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of deaths","@death_counts"],["% mortality","@death_percent"]]},"id":"1059","type":"HoverTool"},{"attributes":{"axis_label":"%","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1063"},"major_label_text_font_size":"10pt","ticker":{"id":"1062"},"y_range_name":"foo"},"id":"1056","type":"LinearAxis"},{"attributes":{},"id":"1062","type":"BasicTicker"},{"attributes":{},"id":"1063","type":"BasicTickFormatter"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1026"},{"id":"1059"}]},"id":"1028","type":"Toolbar"},{"attributes":{"data":{"death_counts":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","1","1","1","1","1","1","1","1","1","1","3","5","6","7","8","8","9","10","11","11","12","14","15","15","15","15","17","18","18","20","22","23","24","24","25","27","27","28","29","30","31","33","35","37","40","44","47","53","61","64","66","71","74","78","81","84","87","94","98","103","111","118","127","133","145","154","160","173","184","197"],"death_percent":["0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","0","4.35","3.45","2.63","2.38","2","1.49","0.81","0.43","0.32","0.24","0.62","0.88","0.97","1.01","1.08","0.96","0.99","1.03","1.02","0.94","1","1.13","1.18","1.13","1.09","1.02","1.12","1.13","1.1","1.19","1.25","1.26","1.27","1.24","1.21","1.25","1.16","1.11","1.05","0.99","0.87","0.81","0.72","0.68","0.67","0.67","0.65","0.66","0.7","0.69","0.68","0.7","0.7","0.69","0.69","0.67","0.66","0.67","0.66","0.66","0.68","0.69","0.72","0.72","0.75","0.76","0.76","0.77","0.78","0.80"],"x":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"selected":{"id":"1052"},"selection_policy":{"id":"1051"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"death_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1038","type":"VBar"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"death_counts"},"width":{"value":0.9},"x":{"field":"x"}},"id":"1037","type":"VBar"},{"attributes":{},"id":"1069","type":"UnionRenderers"},{"attributes":{},"id":"1070","type":"Selection"},{"attributes":{"text":"Day 0 (first detected case): 07 March 2020","x":1,"y":192},"id":"1002","type":"Label"},{"attributes":{"text":"Number of deaths (Cumulative) and % mortality rate","text_font_size":{"value":"15pt"}},"id":"1004","type":"Title"},{"attributes":{"end":5},"id":"1035","type":"Range1d"},{"attributes":{"data_source":{"id":"1041"},"glyph":{"id":"1042"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1043"},"selection_glyph":null,"view":{"id":"1045"},"y_range_name":"foo"},"id":"1044","type":"GlyphRenderer"},{"attributes":{"below":[{"id":"1014"}],"center":[{"id":"1016"},{"id":"1020"},{"id":"1054"},{"id":"1002"}],"extra_y_ranges":{"foo":{"id":"1035"}},"left":[{"id":"1017"}],"plot_height":350,"plot_width":700,"renderers":[{"id":"1039"},{"id":"1044"}],"right":[{"id":"1056"}],"title":{"id":"1004"},"toolbar":{"id":"1028"},"x_range":{"id":"1006"},"x_scale":{"id":"1010"},"y_range":{"id":"1008"},"y_scale":{"id":"1012"}},"id":"1003","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1048","type":"CategoricalTickFormatter"},{"attributes":{"factors":["07-Mar","08-Mar","09-Mar","10-Mar","11-Mar","12-Mar","13-Mar","14-Mar","15-Mar","16-Mar","17-Mar","18-Mar","19-Mar","20-Mar","21-Mar","22-Mar","23-Mar","24-Mar","25-Mar","26-Mar","27-Mar","28-Mar","29-Mar","30-Mar","31-Mar","01-Apr","02-Apr","03-Apr","04-Apr","05-Apr","06-Apr","07-Apr","08-Apr","09-Apr","10-Apr","11-Apr","12-Apr","13-Apr","14-Apr","15-Apr","16-Apr","17-Apr","18-Apr","19-Apr","20-Apr","21-Apr","22-Apr","23-Apr","24-Apr","25-Apr","26-Apr","27-Apr","28-Apr","29-Apr","30-Apr","01-May","02-May","03-May","04-May","05-May","06-May","07-May","08-May","09-May","10-May","11-May","12-May","13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"id":"1006","type":"FactorRange"},{"attributes":{},"id":"1050","type":"BasicTickFormatter"},{"attributes":{"end":207},"id":"1008","type":"Range1d"},{"attributes":{"axis_label":"Day","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1048"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1057"}},"id":"1014","type":"CategoricalAxis"},{"attributes":{},"id":"1010","type":"CategoricalScale"},{"attributes":{},"id":"1012","type":"LinearScale"}],"root_ids":["1003"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1193').textContent;
                  var render_items = [{"docid":"41fd2329-0e7a-453e-a6bc-bc40b3b2f7db","root_ids":["1003"],"roots":{"1003":"4d66c5e5-d30b-45cf-9921-430aac3a3dea"}}];
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
 <div class="bk-root" id="f332fcc8-e81e-4838-b754-115fb25911fd" data-root-id="1043"></div>
   <script type="application/json" id="1132">
          {"07888c41-e99a-4a96-b79a-ab5d4107f314":{"roots":{"references":[{"attributes":{"axis_label":"No. of Cases","axis_label_text_font":"times","axis_label_text_font_size":"15pt","axis_label_text_font_style":"normal","formatter":{"id":"1047"},"major_label_text_font_size":"10pt","ticker":{"id":"1017"}},"id":"1016","type":"LinearAxis"},{"attributes":{"js_property_callbacks":{"change:value":[{"id":"1041"}]},"options":["Ariyalur","Chengalpattu","Chennai","Coimbatore","Cuddalore","Dharmapuri","Dindigul","Erode","Kallakurichi","Kancheepuram","Kanyakumari","Karur","Krishnagiri","Madurai","Nagapattinam","Namakkal","Nilgiris","Perambalur","Pudukottai","Ramnad","Ranipet","Salem","Sivagangai","Tenkasi","Thanjavur","Theni","Thirupathur","Thiruvallur","Thiruvannamalai","Thiruvarur","Thoothukudi","Tirunelveli","Tiruppur","Trichy","Vellore","Villupuram","Virudhunagar"],"title":"Select District:","value":"Ariyalur","width":140},"id":"1042","type":"Select"},{"attributes":{},"id":"1017","type":"BasicTicker"},{"attributes":{"axis":{"id":"1016"},"dimension":1,"ticker":null},"id":"1019","type":"Grid"},{"attributes":{"overlay":{"id":"1026"}},"id":"1022","type":"BoxZoomTool"},{"attributes":{},"id":"1025","type":"HelpTool"},{"attributes":{},"id":"1049","type":"Selection"},{"attributes":{},"id":"1020","type":"PanTool"},{"attributes":{},"id":"1021","type":"WheelZoomTool"},{"attributes":{},"id":"1050","type":"UnionRenderers"},{"attributes":{},"id":"1023","type":"SaveTool"},{"attributes":{},"id":"1024","type":"ResetTool"},{"attributes":{"data":{"x":["13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"],"y":["335","335","153","34","25","27","10","10","7","7","7","8","8","9","7","7","10","10","10","15","11"],"y0":["335","335","153","34","25","27","10","10","7","7","7","8","8","9","7","7","10","10","10","15","11"],"y1":["345","358","377","389","306","344","365","423","416","455","481","518","568","589","482","519","545","499","555","596","634"],"y10":["9","14","18","20","20","27","32","28","25","24","21","23","26","30","31","31","32","35","34","34","36"],"y11":["12","13","12","11","27","28","34","27","25","25","25","25","14","13","13","7","4","5","5","5","5"],"y12":["20","20","20","18","20","20","2","3","3","4","3","3","4","6","5","6","6","7","8","8","8"],"y13":["38","47","54","56","51","53","53","62","80","111","111","114","111","109","99","94","94","99","102","100","92"],"y14":["3","3","3","4","5","5","6","6","6","5","3","3","3","0","1","3","3","8","9","9","12"],"y15":["16","16","0","0","0","0","0","","0","0","0","0","0","0","0","0","0","0","0","4","4"],"y16":["3","3","3","3","3","3","3","2","2","2","1","1","1","1","1","0","0","0","0","1","0"],"y17":["125","124","109","109","106","106","48","48","26","6","5","4","4","4","4","0","0","1","2","3","3"],"y18":["5","5","5","5","5","5","5","7","8","11","12","13","13","13","14","15","14","9","10","8","8"],"y19":["14","9","9","9","9","15","17","17","17","25","25","28","33","33","34","28","27","40","45","33","32"],"y2":["4470","4834","5114","5017","5220","5460","5691","5345","5681","5523","5865","5653","5911","6056","6307","6351","6353","6539","6781","7450","7880"],"y20":["35","35","36","39","35","37","38","26","28","29","29","25","28","20","20","17","15","13","14","18","15"],"y21":["5","5","0","0","9","14","14","14","14","14","17","17","23","33","33","67","62","99","123","139","152"],"y22":["0","1","1","10","14","14","14","13","16","16","3","4","4","3","5","4","4","4","5","6","7"],"y23":["21","20","22","26","24","30","28","27","33","32","33","33","33","32","31","29","24","25","23","23","22"],"y24":["23","23","18","18","10","10","9","10","14","14","13","16","17","17","16","15","10","12","12","16","17"],"y25":["28","29","35","35","35","44","45","47","51","49","50","50","52","43","31","29","23","21","21","15","14"],"y26":["10","10","10","0","8","9","7","7","4","4","4","4","4","5","4","4","4","5","4","5","8"],"y27":["406","410","429","348","363","382","380","395","413","424","426","452","429","312","345","339","332","327","334","359","398"],"y28":["115","123","126","133","110","114","114","116","109","98","103","107","148","152","171","210","244","252","273","283","296"],"y29":["3","3","3","3","3","3","2","2","0","3","3","5","6","6","9","9","9","13","14","13","13"],"y3":["0","0","0","0","0","0","0","1","0","0","0","0","0","0","0","1","0","0","0","5","5"],"y30":["9","11","20","28","40","55","60","82","104","108","111","119","129","128","114","110","93","87","89","79","126"],"y31":["35","51","72","116","129","141","155","163","164","177","187","182","197","175","154","174","177","168","140","105","89"],"y32":["0","0","0","0","0","0","0","","0","0","0","0","0","0","0","0","0","0","0","0","0"],"y33":["11","11","11","10","5","5","6","2","2","6","6","9","9","9","11","10","11","15","18","18","25"],"y34":["13","13","13","12","11","11","7","7","6","9","5","5","5","8","6","8","8","8","8","12","12"],"y35":["251","251","176","153","30","34","31","38","26","24","24","24","24","22","25","35","34","28","26","34","24"],"y36":["13","12","14","13","16","17","18","24","29","52","53","54","71","70","69","69","70","63","65","66","65"],"y4":["384","384","378","164","157","55","42","38","19","15","15","17","12","21","22","26","28","32","40","40","41"],"y5":["4","4","4","4","3","1","1","1","1","0","0","0","1","3","3","3","3","3","3","3","3"],"y6":["31","31","30","25","23","25","19","20","25","26","26","22","22","21","21","25","17","17","16","21","22"],"y7":["0","0","0","0","0","0","0","1","0","1","1","1","1","1","1","1","2","2","1","1","3"],"y8":["51","51","47","64","56","61","67","54","62","60","60","75","67","60","134","124","132","134","135","125","114"],"y9":["132","97","104","81","78","95","87","98","106","98","108","132","138","132","129","144","155","164","173","164","177"]},"selected":{"id":"1049"},"selection_policy":{"id":"1050"}},"id":"1001","type":"ColumnDataSource"},{"attributes":{"args":{"source":{"id":"1001"}},"code":"\n        var data = source.data;\n        var f = cb_obj.value\n        if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Ariyalur\") {source.data['y'] = source.data['y0'];}\n        else if(f==\"Chengalpattu\") {source.data['y'] = source.data['y1'];}\n        else if(f==\"Chennai\") {source.data['y'] = source.data['y2'];}\n        else if(f==\"Coimbatore\") {source.data['y'] = source.data['y3'];}\n        else if(f==\"Cuddalore\") {source.data['y'] = source.data['y4'];}\n        else if(f==\"Dharmapuri\") {source.data['y'] = source.data['y5'];}\n        else if(f==\"Dindigul\") {source.data['y'] = source.data['y6'];}\n        else if(f==\"Erode\") {source.data['y'] = source.data['y7'];}\n        else if(f==\"Kallakurichi\") {source.data['y'] = source.data['y8'];}\n        else if(f==\"Kancheepuram\") {source.data['y'] = source.data['y9'];}\n        else if(f==\"Kanyakumari\") {source.data['y'] = source.data['y10'];}\n        else if(f==\"Karur\") {source.data['y'] = source.data['y11'];}\n        else if(f==\"Krishnagiri\") {source.data['y'] = source.data['y12'];}\n        else if(f==\"Madurai\") {source.data['y'] = source.data['y13'];}\n        else if(f==\"Nagapattinam\") {source.data['y'] = source.data['y14'];}\n        else if(f==\"Namakkal\") {source.data['y'] = source.data['y15'];}\n        else if(f==\"Nilgiris\") {source.data['y'] = source.data['y16'];}\n        else if(f==\"Perambalur\") {source.data['y'] = source.data['y17'];}\n        else if(f==\"Pudukottai\") {source.data['y'] = source.data['y18'];}\n        else if(f==\"Ramnad\") {source.data['y'] = source.data['y19'];}\n        else if(f==\"Ranipet\") {source.data['y'] = source.data['y20'];}\n        else if(f==\"Salem\") {source.data['y'] = source.data['y21'];}\n        else if(f==\"Sivagangai\") {source.data['y'] = source.data['y22'];}\n        else if(f==\"Tenkasi\") {source.data['y'] = source.data['y23'];}\n        else if(f==\"Thanjavur\") {source.data['y'] = source.data['y24'];}\n        else if(f==\"Theni\") {source.data['y'] = source.data['y25'];}\n        else if(f==\"Thirupathur\") {source.data['y'] = source.data['y26'];}\n        else if(f==\"Thiruvallur\") {source.data['y'] = source.data['y27'];}\n        else if(f==\"Thiruvannamalai\") {source.data['y'] = source.data['y28'];}\n        else if(f==\"Thiruvarur\") {source.data['y'] = source.data['y29'];}\n        else if(f==\"Thoothukudi\") {source.data['y'] = source.data['y30'];}\n        else if(f==\"Tirunelveli\") {source.data['y'] = source.data['y31'];}\n        else if(f==\"Tiruppur\") {source.data['y'] = source.data['y32'];}\n        else if(f==\"Trichy\") {source.data['y'] = source.data['y33'];}\n        else if(f==\"Vellore\") {source.data['y'] = source.data['y34'];}\n        else if(f==\"Villupuram\") {source.data['y'] = source.data['y35'];}\n        else if(f==\"Virudhunagar\") {source.data['y'] = source.data['y36'];}\n        source.change.emit();\n\n    "},"id":"1041","type":"CustomJS"},{"attributes":{"children":[{"id":"1042"},{"id":"1002"}]},"id":"1043","type":"Row"},{"attributes":{"source":{"id":"1001"}},"id":"1038","type":"CDSView"},{"attributes":{"bottom_units":"screen","fill_alpha":0.5,"fill_color":"lightgrey","left_units":"screen","level":"overlay","line_alpha":1.0,"line_color":"black","line_dash":[4,4],"line_width":2,"render_mode":"css","right_units":"screen","top_units":"screen"},"id":"1026","type":"BoxAnnotation"},{"attributes":{"active_drag":"auto","active_inspect":"auto","active_multi":null,"active_scroll":"auto","active_tap":"auto","tools":[{"id":"1020"},{"id":"1021"},{"id":"1022"},{"id":"1023"},{"id":"1024"},{"id":"1025"},{"id":"1039"}]},"id":"1027","type":"Toolbar"},{"attributes":{"data_source":{"id":"1001"},"glyph":{"id":"1035"},"hover_glyph":null,"muted_glyph":null,"nonselection_glyph":{"id":"1036"},"selection_glyph":null,"view":{"id":"1038"}},"id":"1037","type":"GlyphRenderer"},{"attributes":{"below":[{"id":"1013"}],"center":[{"id":"1015"},{"id":"1019"}],"left":[{"id":"1016"}],"plot_height":350,"plot_width":550,"renderers":[{"id":"1037"}],"title":{"id":"1003"},"toolbar":{"id":"1027"},"x_range":{"id":"1005"},"x_scale":{"id":"1009"},"y_range":{"id":"1007"},"y_scale":{"id":"1011"}},"id":"1002","subtype":"Figure","type":"Plot"},{"attributes":{},"id":"1011","type":"LinearScale"},{"attributes":{"fill_alpha":{"value":0.1},"fill_color":{"value":"#1f77b4"},"line_alpha":{"value":0.1},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1036","type":"VBar"},{"attributes":{"fill_color":{"value":"#1f77b4"},"line_color":{"value":"#1f77b4"},"top":{"field":"y"},"width":{"value":0.8},"x":{"field":"x"}},"id":"1035","type":"VBar"},{"attributes":{},"id":"1045","type":"CategoricalTickFormatter"},{"attributes":{"callback":null,"tooltips":[["DATE","@x"],["No. of cases","@y"]]},"id":"1039","type":"HoverTool"},{"attributes":{"text":"Number of active cases in the last 21 days","text_font_size":{"value":"12pt"}},"id":"1003","type":"Title"},{"attributes":{},"id":"1009","type":"CategoricalScale"},{"attributes":{},"id":"1014","type":"CategoricalTicker"},{"attributes":{"factors":["13-May","14-May","15-May","16-May","17-May","18-May","19-May","20-May","21-May","22-May","23-May","24-May","25-May","26-May","27-May","28-May","29-May","30-May","31-May","01-Jun","02-Jun"]},"id":"1005","type":"FactorRange"},{"attributes":{"axis_label_text_font_size":"15pt","formatter":{"id":"1045"},"major_label_orientation":1.5707963267948966,"major_label_text_font_size":"10pt","ticker":{"id":"1014"}},"id":"1013","type":"CategoricalAxis"},{"attributes":{},"id":"1007","type":"DataRange1d"},{"attributes":{"axis":{"id":"1013"},"ticker":null},"id":"1015","type":"Grid"},{"attributes":{},"id":"1047","type":"BasicTickFormatter"}],"root_ids":["1043"]},"title":"Bokeh Application","version":"2.0.1"}}
        </script>
        <script type="text/javascript">
          (function() {
            var fn = function() {
              Bokeh.safely(function() {
                (function(root) {
                  function embed_document(root) {
                    
                  var docs_json = document.getElementById('1132').textContent;
                  var render_items = [{"docid":"07888c41-e99a-4a96-b79a-ab5d4107f314","root_ids":["1043"],"roots":{"1043":"f332fcc8-e81e-4838-b754-115fb25911fd"}}];
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


04 April 2020

This is day 10 of the lock down which is in effect because of the worldwide COVID19 outbreak. I'm in the last stretch of my doctoral research and I have hit a roadblock. Using my laptop and remote computing, some progress was possible in the last 10 to 15 days. But, I have to admit that this has been a difficult situation for me to focus on my research. Meanwhile, the outbreak, though saddening, is intriguing phenomenon for any researcher. Tons of data on the outbreak is pouring in from all over the world everyday. So, I have decided to practice some data visualization technqiues making use of the data. I will be using python language (v3.8.2) and the <a href= "https://bokeh.org/" >Bokeh library </a>, in particular, to visualize and then embed the results here. The dataset I will be working on is the COVID19 outbreak data for my home state of Tamil Nadu. The source is the <a href="https://stopcorona.tn.gov.in/">official website</a> of the Tamil Nadu health department dedicated for addressing the COVID19 outbreak. Hopefully, the source is regulary updated so that I can also regularly update the visualizations. (The plots are best viewed in a desktop)


Update: 09 April 2020

There is a major concern that India is not carrying out enough tests. The state of Tamil Nadu which has a population of 82 million has conducted a total of only 7267 tests till 09 April 2020. To get some perspective, South Korea, a country which is being praised universally for its immaculate management of the COVID19 crisis has a population of about 52 million. The tests per million (TPM) is one of the highest and is seen as key to their success by experts. Tamil Nadu crossed the 100 cases mark on 31st March 2020. From 1st April 2020 to 9th April 2020, the number of tests conducted were 4913. The low number of tests conducted in Tamil Nadu makes it difficult to say for certain the degree of tranmission within the population. Also, a majority of the tests carried out was focussed on a single source group. With the arrival of nearly 50,000 rapid antibody test kits expected soon, we will hopefully get a clearer picture in the coming days. With the increase in number of tests, plateauing or decreasing of the %positive trend would be a welcome sight.

Update: 27 April 2020

This is day 34 of the national lockdown. Although some recommendations for easing restrictions has been made by the central governemnt recently, this is not applicable for Chennai and also to pretty much the whole of Tamil Nadu because of number of zones considered as "hot spots". I have made changes to the third plot above after more clarifications emerged from the Tamil Nadu government. One of the important clarifications being the number of repeat samples now available. So, earlier I had calculated the %positive cases from the total samples collected which is inaccurate. Now, in the updated plot, %positive cases is calculated from the number of unique samples processed. The unique samples processed is obtained from subtracting the repeat samples and the samples under process from the total samples collected. I have also included the % active positive cases. This value excludes those discharged after recovery and those deceased. I will soon add more graphs visualizing other data such as recovered and deceased numbers. 

Update: 05 May 2020

There has been some relaxations in the lockdown restrictions but this is accomponied by record daily cases in India. Tamil Nadu is turning out to be a major contributor to the total national count. There are many reasons being debated non-stop in the media for the rise in the number of cases in the recent days. So, I'm not going to get into that. Back to the data visualisations, I've added another plot - the cumulative positive cases in the last 14 days for every district in Tamil Nadu. A selection menu is included for choosing the district. I was struggling  to get this plot right (it is not perfect yet) for several hours stretched over several days. I finally got it to work yesterday. 

Update: 07 May 2020

I have added the death statistics and % mortality plot. Also, I have expanded the district wise trends graph to include the last 21 days total cases. This is in accordance to the the stipulated 21 day duration prescibed by the central government for a district to move from "orange" zone to "green" zone if no new cases are reported in this period.

Update: 23 May 2020

I have updated the plots after nearly ten days.  I was a little busy writing my thesis. A lot has happened in this period. More restrictions are lifted and people stuck during the lockdown are returning to their homes via special trains and planes. As for the outbreak itself, it is almost becoming an afterthough in peoples' minds. But the reality is anything but as the number of cases is rapidly increasing in India as well as in Tamil Nadu. Looking at the data, there was a slight wobble in the number of tests because there was a brief reduction in the tests conducted for a couple of days (around 8K-10K) and then it went to be previous numbers (around 12K tests). Experts are crying out for ramping up testing but it is not happening. The gap between %total positive and %total active is increasing mainly due to revised discharge guidelines released by ICMR which has lessened the stringency of discharge criterion.  Today (23 May 2020), the number of deaths went past 100 but the %mortality has plateaued to about 0.65%.

P. S.

Apart from the official Python and Bokeh documentations and numerous google searches to check and correct minor issues in the python code, there are a few sources which helped me a lot in writing this code. I'm listing them below:

*   <a href="https://stackoverflow.com/questions/49722791/python-bokeh-vbar-hover-tool"> Stackoverflow question on adding hovertool to bargraph </a>

* <a href="https://stackoverflow.com/questions/25050311/extract-first-item-of-each-sublist"> Stack Overflow question on list comprehension </a>

* Stack Overflow questions <a href="https://stackoverflow.com/questions/25199665/one-chart-with-two-different-y-axis-ranges-in-bokeh/30914348#30914348">(1) </a><a href = "https://stackoverflow.com/questions/29267141/bokeh-add-label-to-second-axis-on-the-right">(2)</a> on adding second axis.



[back](./)


### Python-Bokeh Data Visualization


I am sharing below the python codes for the data visualiztion of the COVID19 outbreak in Tamil Nadu in my previous post. Please note that I'm not a professional programmer and so, the codes could be considered crude by expert coders. I hope my codes don't scare them too much. The programs are meant to just about work and far from being memory-efficient. So, tread with caution! All of the plots have interactive tooltips on hovering. The last plot uses a dropdown selection menu which allows users to select an option among many and the appropriate graph appears. The data along with the codes can also be found here: <a href="https://github.com/aksaba/MyCodes/tree/master/Py/DataVisualisation/TNCOVID19"> Data and Codes </a>


Cumulative and Daily cases - bar graphs

<div style="height:600px;width:850px;border:1px solid #ccc;font-family:'Courier New';overflow:auto">
<pre><code>
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
</code> </pre></div>


Total samples tested with %total positive cases and %total active cases - three line plots in the same graph along with a secondary y-axis

<div style="height:600px;width:850px;border:1px solid #ccc;font-family:'Courier New';overflow:auto">
<pre><code>
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
</code> </pre></div>

Number of deaths and %mortality- bar plot and line plot in the same graph, secondary y-axis

<div style="height:600px;width:850px;border:1px solid #ccc;font-family:'Courier New';overflow:auto">
<pre><code>
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
</code> </pre></div>


District wise trends - multiple graphs with selection dropdown menu

<div style="height:600px;width:850px;border:1px solid #ccc;font-family:'Courier New';overflow:auto">
<pre><code>
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
</code> </pre></div>


[back](./)
