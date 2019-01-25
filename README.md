# RStoCSV

Easy to use program that converts JSON data exports from [Robot Scouter](https://github.com/SUPERCILEX/Robot-Scouter) to CSV for easy analysis in programs like Tableau and Excel!


## Installation
Make sure you have [Git](https://git-scm.com/) installed

1. In your terminal of choice, navigate to where you want the folder to be installed. [Click here if that was gibberish](https://www.davidbaumgold.com/tutorials/command-line/).
2. Enter the following command:
`git clone https://github.com/will-hou/RStoCSV.git`
3. You're good to go! RStoCSV is installed locally on your computer!


## Usage
1. Make sure you're in the RStoCSV directory
2. To convert your Robot Scouter JSON file to CSV, enter:

`python convert.py -p [path_to_your_json_file]` without brackets and path_to_your_json_file being the path to your JSON file
 
 3. A new `.csv` file with the same name will be made in the same directory
 
### Example Usage
  Input:
  `python convert.py -p C:/Users/William/Scouting_Data/scout.json`
  
  Output:
  `C:/Users/William/Scouting_Data/scout.csv`
 
 
 
 
 
 
  
 ## Happy Analyzing :D
