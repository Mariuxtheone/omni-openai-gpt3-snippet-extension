# NVIDIA Omniverse OpenAI GPT-3 Snippet Extension

This is an Extension that adds a simple snippet UI to NVIDIA Omniverse which allows you to generate GPT-3 based snippets.

## 1) Dependencies

In order to use this extension, you will need to install the following dependencies:

- openai python library: `pip install openai`
- pyperclip: `pip install pyperclip`

## 2) Installation

1) Install the Extension in your Omniverse app.
2) We need to create a folder to include the OPEN AI API key and the path to the main Python modules repository on our device, since Omniverse doesn't use the Python global PYTHONHOME and PYTHONPATH.
3) To do this, in the omni\openai\snippet\ folder, create a new file called `apikeys.py`
4) in the `apikeys.py` file, add the following lines:

```   
apikey = "YOUR_OPENAI_API_KEY_GOES_HERE"
pythonpath = "The file path where you have installed your main python modules"
```

so `apikeys.py` should look like this:

```
apikey = "sk-123Mb38gELphag234GDyYT67FJwa3334FPRZQZ2Aq5f1o" (this is a fake API key, good try!)
pythonpath = "C:/Users/yourusername/AppData/Local/Packages/PythonSoftwareFoundation.Python.3.10_qbz5n2kfra8p0/LocalCache/local-packages/Python310/site-packages"
```

## 3) Enable and Usage

To use the extension, enable it from the Extension Window and then click the "Generate Snippet" button. The generated snippet will be copied to your clipboard and you can past anywhere you want.

## 4) IMPORTANT DISCLAIMER
1) OpenAI is a third party API and you will need to create an account with OpenAI to use it. Consider that there's a cost associated with using the API.

2) The extension by default generate snippets up to 40 Tokens. If you want to generate more tokens, you will need to edit the variable `openaitokensresponse`





