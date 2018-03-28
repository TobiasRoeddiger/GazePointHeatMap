# Gaze Point Heat Map
Easy to use command line based tool to generate a gaze point heat map from a csv file. 👁️

## Usage
Install the required dependencies from the command line.

```bash
pip install -r requirements.txt
```

**This tool was created based on Python 2.7. Make sure you are on that Python version to avoid problems.**

Run the script from the command line.
```bash  
python gazeheatplot.py gaze-data.csv 1440 900 [-a 0.6] [-o output-name] [-b /Me/bg-image.png] [-n 200] [-sd 33]
``` 

### Data Format
Each line contains at least the X- and Y-values. If you have fixation data and want to take the duration into account you can add it to the end of each row. The data has to be formatted in the [CSV format](https://en.wikipedia.org/wiki/Comma-separated_values) (comma-separated values).

| X | Y | Duration (optional) |
|:-:|:-:|:-------------------:|
|123|654|         226         |
|134|662|         234         |
|...|...|         ...         |

### Shortcut and Additional Arguments

```
GENERAL ARGUMENTS:
-h                    --help                                 show help message and exit

REQUIRED ARGUMENTS:
input-path                                                   path to the csv input
display-width                                                an integer representing the display width
display-height                                               an integer representing the display height

OPTIONAL ARGUMENTS:
[-a ALPHA             --alpha ALPHA                          alpha of the gaze overlay                 ]
[-o OUTPUT_NAME       --output-name OUTPUT_NAME              name of the output file                   ]
[-b BACKGROUND_IMAGE  --background-image BACKGROUND_IMAGE    path to the background image              ]

ADVANCED OPTIONAL ARGUMENTS:
[-n  N_GAUS_MATRIX    --n-gaussian-matrix N_GAUSS_MATRIX     width and height of gaussian matrix       ]
[-sd STAND_DEVIATION  --standard-deviation STAND_DEVIATION   standard deviation of gauss distribution  ]
```
**Note:** To add a background image make sure to *provide the whole path and only png images without an alpha channel which are not larger than the provided display width and display height*.

## Results
![Example Output](https://github.com/r0ehre/GazeHeatPlot/blob/master/Example%20Output/output.png)

 ## Attribution
 The script is based on the heat map plotter of [PyGaze](http://www.pygaze.org).
