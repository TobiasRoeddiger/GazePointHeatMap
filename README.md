# GazeHeatPlot
Simple Python command line based script to generate a gaze heatmap from a csv file. 👁️

## Usage
Install the required dependencies over the command line.
```bash
pip install -r requirements.text
```

Run the script from the command line.
```bash  
python gazeheatplot.py --input-path gaze-data.csv --display-width 1440 --display-height 900
``` 

### Shortcut and Additional Arguments
```bash
 -i INPUT_PATH        --input-path INPUT_PATH           path to the csv input
 -dw DISPLAY_WIDTH    --display-width DISPLAY_WIDTH     an integer representing the display width
 -dh DISPLAY_HEIGHT   --display-height DISPLAY_HEIGHT   an integer representing the display height
 [-a ALPHA            --alpha ALPHA                     alpha of the gaze overlay]
 [-o OUTPUT_NAME      --output-name OUTPUT_NAME         name of the output file]
 ```
