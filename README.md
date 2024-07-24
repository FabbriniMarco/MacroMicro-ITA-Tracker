<div align=center>
  <img width="196" alt="Circle logo" src="https://github.com/user-attachments/assets/46f5dbf9-aee4-4d8d-a1d4-bbe468bfdfcf" height="186">
</div>

# MacroMicro-ITA-Tracker: Analyze Diets with Italian Food Tables

MacroMicro-ITA-Tracker is a free open-source nutritional data calculator tool that helps researchers and clinicians to analyze the nutritional content of Italian meals. The food tables have been downloaded from the "CREA Centro di ricerca Alimenti e Nutrizione" (Italian Council for Agricultural Research and Analysis of Agricultural Economic) web page: https://www.alimentinutrizione.it/sezioni/tabelle-nutrizionali and https://www.alimentinutrizione.it.

This tool allows users to select foods from a comprehensive list of 900 foods, specify the quantity in grams, and get detailed information about the macro and micronutrients present in the dietary intake.

<div align=center>
  <img width="377" alt="Screenshot 1" src="https://github.com/user-attachments/assets/e4362888-75c9-49d4-877b-bdd415b5390d" height="420">
  <img width="377" alt="Screenshot 2" src="https://github.com/user-attachments/assets/15b6256f-c3d7-4663-923f-ef995f35de69" height="420">
</div>

<br>
<br>

## Table of Contents

- [Features](#features)
- [Installation and usage](#installation-and-usage)
- [Add food and export data](#add-food-and-export-data)
- [Data Sources](#data-sources)
- [Citation](#citation)
- [License](#license)
  
<br>
<br>

## Features

- **Extensive Food Database**: Includes nutritional data for 900 foods. <br>
- **Detailed Nutritional Information**: Provides information on both macro and micronutrients for selected foods. <br>
- **Search Functionality**: Allows users to search for foods by name. <br>
- **Quantity Specification**: Users can specify the quantity of each food item to get proportionate nutritional information. <br>
- **Data Export**: Users can export the aggregated nutritional data to a TSV file. It's up to user choice wether to generate an export per-meal, per-daily intake or whatever time span. <br>
- **Clear Data**: Option to clear all inputs and start a new analysis. <br>
- **Dual Language**: The database based on italian foods can be consulted both with Italian and English food names, for practicity. <br>
- **Info and Help Links**: Provides links to usage instructions and proper citation to the original data. <br>


<br>
<br>

## Installation and usage

### Windows user: portable pre-built .exe file
If you are a Windows user, you just need to fetch the NutriTableCREAtion.exe file either cloning this repo or downloading from the [Release](https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker/releases) section.
Once downloaded simply double-click the .exe file. That's it!
The .exe file has been signed, therefore no warnings related to unknown developers should appear when opening the program.
<br>

### Linux and MacOS users: run the python script
#### Prerequisites
- Python 3.7 or higher
- `ttkbootstrap` library
- `tkinter` library (usually comes pre-installed with Python)

Use pip to install the required libraries:
```sh
py -m pip install tk
py -m pip install ttkbootstrap
```

Clone this repository and navigate to the project directory:

```sh
git clone https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker.git
cd MacroMicro-ITA-Tracker
python MacroMicro-ITA-Tracker.py
```

You can also download the tarball archive from the [Release](https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker/releases) section and decompress it.

```sh
wget https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker/releases/download/v1.0/MacroMicro-ITA-Tracker.tar.gz
tar -zxvf MacroMicro-ITA-Tracker.tar.gz
cd MacroMicro-ITA-Tracker
python MacroMicro-ITA-Tracker.py
```

<br>
<br>

## Add food and export data

1. Select Food: Use the dropdown menu to select a food item. You can also search for a food by typing part of its name in the search bar. <br>
2. Enter Quantity: Enter the quantity (in grams) of the selected food. <br>
3. Add Food: Click the "Add Food" button to add the food to your list. The added foods along with their quantities will be displayed in a list. <br>
4. Delete: Next to each added food in the list, a "Delete" button is displayed, allowing (upon a second confirm) to remove the corresponding item, in case a food is added by mistake. <br>
5. Duplicate: Next to each "Delete" button, you will find a "Duplicate" button. Once pressed, it allows to duplicate the given food (with the same amount) to speed up recording repeated daily-,weekly- intakes.
6. Export Data: Once done adding all the foods, click the "Export Data" button to save the nutritional information to a TSV file. <br>
7. Wipe Data: Click the "Wipe Data" button to clear all inputs and start a new analysis. You will be prompted to confirm this action. <br>
<br>

Info: Click the "Info" button for details about the program, including version, maintainer contact, and reference links. <br>
External Links: Use the "Github" button to visit this project's GitHub repository. <br>


Food data in the CREA food tables are reported with macronutrients in absolute quantities (grams) and micronutrients in percentages based on the Protein and Lipid fractions. When a food item is added to the list, the tool calculates the relative macronutrient content based on the input quantity. This relative amount is then used to determine the precise absolute quantity of micronutrients according to the percentages from the food tables. The tool generates a TSV table that shows the total amounts of both micro and macronutrients in absolute quantities (grams, milligrams, micrograms, millimoles, or kJ/kcal for energy).


<br>
<br>

## Data Sources
The nutritional data used by this tool is sourced from the CREA food tables, which can be consulted at the original source.
Reference is: CREA Food and Nutrition Research Center, Web page: https://www.crea.gov.it/alimenti-e-nutrizione and Web page: https://www.alimentinutrizione.it


<br>
<br>


## Citation
If you use this tool, please cite both the tool and the CREA, Centro di ricerca Alimenti e la Nutrizione. 

```diff
@Manual{,
  title = {MacroMicro-ITA-Tracker: Analyze Diets with Italian CREA Food Tables},
  author = {Marco Fabbrini},
  year = {2024},
  note = {Version v1.0},
  url = {https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker.git},
}
```
``` diff
@Manual{,
  title = {TABELLE DI COMPOSIZIONE DEGLI ALIMENTI, CREA AN, Aggiornamento 2019},
  author = {CREA-AN},
  year = {2019},
  url = {https://www.alimentinutrizione.it/tabelle-di-composizione-degli-alimenti},
}
```

Example: 
> Fabbrini, M. (2024) 'MacroMicro-ITA-Tracker: Analyze Diets with Italian CREA Food Tables'. Available on Github: https://github.com/FabbriniMarco/MacroMicro-ITA-Tracker.git
<br>

> CREA-AN (2019) 'TABELLE DI COMPOSIZIONE DEGLI ALIMENTI, CREA AN, Aggiornamento 2019'. Website: https://www.alimentinutrizione.it/tabelle-di-composizione-degli-alimenti

<br>
<br>

## License

This project is licensed under the custom MacroMicro-ITA-Tracker License. You are free to use, copy, and distribute the software for private, personal, and academic research purposes.

**Restrictions:**
- No commercial use
- No modifications
- No patent use

For full licensing details, see the [LICENSE](./LICENSE) file.

For any use cases not covered under this license, please contact the maintainer and CREA, Centro di ricerca Alimenti e la Nutrizione.

