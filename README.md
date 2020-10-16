# GDIENT

**A simple JavaScript library to output gradients.**

This work is still under progress.

**Usage**
1. Add your gradients in the JSON file following this format:
   ```
   {
    "gradient-list" : 
        {
            "YOUR-GRADIENT-NAME": [
                "frames": [
                    {   
                        "type": "linear-gradient",
                        "direction": "YOUR GRADIENT DIRECTION",
                        "colors": "COLOR-LIST (lower case, seperated by comma)"
                    }
                    ,{   
                        "type": "linear-gradient",
                        "direction": "YOUR GRADIENT DIRECTION",
                        "colors": "COLOR-LIST (lower case, seperated by comma)"
                    }
            ]
        }
   }
   ```
   All of the properties and values is following CSS syntax.
   For gradient type, there's only linear gradient atm.


2. Run the function (Event Listener etc) `gdient()` with all the needed parameters.


    `gdient(sourceFile, targetElement, gradient, frameDuration, gradientDuration)`
    - **sourceFile** - *Location of gdient JSON file (local or server). Must include .json extension*
    - **targetElement** - *Element that will output the gradient*
    - **gradient** - *Gradient name in JSON file*
    - **frameDuration** - *Duration of each frame (in seconds) . Min 1 second. Only for infinite gradientDuration*
    - **gradientDuration** - *Duration of a gradient (in seconds) . For infinite duration use 'i'*



**DEMO:** [https://github.hanisirfan.xyz/gdient/demo.html](https://github.hanisirfan.xyz/gdient/demo.html)

I don't know who ever need to use this thing but well ¯\_(ツ)_/¯