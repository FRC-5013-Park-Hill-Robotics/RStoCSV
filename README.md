# RStoCSV

Easy to use program that converts JSON data exports from [Robot Scouter](https://github.com/SUPERCILEX/Robot-Scouter) to CSV for easy analysis in programs like Tableau and Excel!


## Installation
Make sure you have: 

* [Git](https://git-scm.com/)
* [Python](https://www.python.org/)
* [PIP](https://pypi.org/project/pip/)

## Python
Download the latest stable version of Python for windows. 
In installation, it will ask you if you want to install PIP (YES)
as well as setting up your environment (YES)
Otherwise, just install the defaults.

1. Enter `pip install -r requirements.txt` to install the necessary dependencies

## GIT 
1. In your terminal of choice, navigate to where you want the folder to be installed. [Click here if that was gibberish](https://www.davidbaumgold.com/tutorials/command-line/).
2. Enter the following command:
`git clone https://github.com/FRC-5013-Park-Hill-Robotics/RStoCSV.git`
3. You're good to go! RStoCSV is installed locally on your computer!

## Usage
1. Make sure you're in the RStoCSV directory.
2. To convert your Robot Scouter JSON file to CSV, enter:

`python convert.py [-f [metric_to_filter by] ] [-t]` With the items in the brackets being optional. Remove the brackets if you want to actually use them.

Optional fields: 

- `-f` Removes any scouts that don't have a value for a specified metric. Enter the name of the metric to filter after the -f flag surrounded by `""`
- `-t` Adds the timestamp of each scout to the CSV file. NOTE: Only use this for data that was exported WITH Robot Scouter version 3.0.0-beta2 or above. You'll get an error otherwise
 
 3. RStoCSV will prompt you to select a Robot Scouter JSON file and will automatically analyze it to find all of the scouted metrics. NOTE: Don't select a file that's located within the local RStoCSV directory.
 4. A new `.csv` file with the same name will be made in the same directory as the original JSON file.
 5. A HTML file called `table.html` will also be created in the local RStoCSV directory for easy visualization.
 
### Example Usage
  Input:
  `python convert.py -f "Scout Name"`
  
  Output:
   ```
   Filtering: Scout Name, With Timestamps: False
   Deleted 31 empty scouts
   Successfully created scout.csv in C:/Users/William/Scouting_Data
   ```
  
 
 
 
 
 
 
 
  
 ## Happy Analyzing :D
