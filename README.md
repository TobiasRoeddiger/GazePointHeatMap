# Gaze Point Heat Map
Simple Python command line based script to generate a gaze point heat map from a csv file. 👁️

## Usage
Install the required dependencies over the command line.
```bash
pip install -r requirements.txt
```

Run the script from the command line.
```bash  
python gazeheatplot.py --input-path gaze-data.csv --display-width 1440 --display-height 900
``` 

### Shortcut and Additional Arguments
```bash
general:
-h                   --help                               show help message and exit

required:
-i INPUT_PATH        --input-path INPUT_PATH              path to the csv input
-dw DISPLAY_WIDTH    --display-width DISPLAY_WIDTH        an integer representing the display width
-dh DISPLAY_HEIGHT   --display-height DISPLAY_HEIGHT      an integer representing the display height

optional:
[-a ALPHA            --alpha ALPHA                        alpha of the gaze overlay                 ]
[-o OUTPUT_NAME      --output-name OUTPUT_NAME            name of the output file                   ]
[-b BACKGROUND_IMAGE --background-image BACKGROUND_IMAGE  path to the background image              ]
```
**Note:** To add a background image make sure to *provide the whole path* and *only png images without an alpha channel and the same resolution as the provided dw and dh*.

### Data Format
|     X         |        Y      |
| ------------- | ------------- |
|     123       |      654      |
|     121       |      657      |
|     ...       |      ...      |

## Results
![Example Output](https://github.com/r0ehre/GazeHeatPlot/blob/master/Example%20Output/output.png)

 ## Appreciation
 The script is based on the heat map plotter of [PyGaze](http://www.pygaze.org).
