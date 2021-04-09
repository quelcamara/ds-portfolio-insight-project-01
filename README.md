<img title="Greener Houses" style = "width:1200px; height:400px" alt="Dreaming House"
src="https://www.rocketmortgage.com/resources-cmsassets/RocketMortgage.com/Article_Images/Large_Images/TypesOfHomes/types-of-homes-hero.jpg">

<h1 align="left">Explanatory Data Analysis to Build some Buy&Sell House Company Insights 🏡</h1>
<p align="left"><a href="https://github.com/quelcamara/startup-success-analysis"><img src="https://img.shields.io/badge/Languages-1-pink"></a> <a href="https://github.com/quelcamara/startup-success-analysis/commits/master"><img src="https://img.shields.io/badge/Last%20Commit-April-red"></a> <a href="https://github.com/quelcamara/startup-success-analysis"><img src="https://img.shields.io/badge/Project%20Status-Finished-lightblue"></a></p>

# Table of Contents
* [About the project](#computer-about-the-project)
* [Overall description](#gear-overall-description)
* [Becoming familiar](#mag_right-becoming-familiar)
  * [Business problem](#business-problem)
  * [Solution planning](#solution-planning)
  * [3 relevant insights](#3-relevant-insights)
  * [Financial results](#financial-results)
  * [Conclusion](#conclusion)
* [Technologies](#hammer_and_wrench-technologies)
* [Setup](#rocket-setup)
  * [Requirements](#requirements)
  * [Installation](#wrench-installation)
  * [Executing online](#globe_with_meridians-executing-online)
  * [Executing via cmd](#game_die-executing-via-cmd)
* [Author](#superhero-author)

## :computer: About the project
This is an insight project developed to be part of my data scientist portfolio. It is basically shaped as an explanatory data analysis to help a fictional company's decision makers to know whether to invest or not in a particular house.

The company, named Greener Houses, is in the market for 8 yrs with a business model focused on buying and selling houses through its digital platform. It is a very technological company and it performs all services based on market analysis decision making.

The main goal was to provide the company useful insights so they can better understand how the market behaves and also their on businesses. This way, they can see the hole picture for the businesses to come.

## :gear: Overall description
The project was divided into 6 sections, each one of them also divided into subtopics. This repository includes the .csv file and a directory where the plots were saved. You will see under the sections:

0. Business and Analysis Understanding:
   - [x] **Business Problem**: states the business questions to be answered along the analysis.
   - [x] **Business Assumptions**: stated the assumptions we make before starting manipulating the dataset. It includes the method we should use in case we need to remove outliers.
   - [x] **Dataset Description**: describes columns and data types for each attribute on the dataset.
   - [x] **Solution Planning**: describes the steps to be taking along the data analysis in order to achieve a good business problem resolution.  
   - [x] **Hypothesis**: states the initial assumptions we made before starting manipulating the dataset. These hypothesis guide us throughout the analysis.

1. Imports:
   - Loads packages, functions and the .csv file into the Jupyter Lab environment. 

2. Descriptive Analysis:
   - It is the stage at which we become familiar with the data. This section includes measures of some statistical variables, such as *mean*, *median*, *mode*, *range*, and so on. It also includes data types, missing and duplicated values checking. Below is an example table for this section:

![image](https://user-images.githubusercontent.com/73648823/114231149-6d975600-9950-11eb-98c8-7da8496c01f9.png)

3. Data Cleaning and Preparation:
   - Under this section, we discuss the need for preparing the dataset by cleaning unwanted data or not, depending on our goal.
   - It also includes a *correlation matrix* plot to state how the attributes relate with one another.

4. Exploratory Data Analysis:
   - [x] **Business Problem Nº1**: contains the resolution for the first business problem.
   - [x] **Business Problem Nº2**: contains the resolution for the second business problem.
   
5. Communicating Results:
   - [x] **Evaluating Hypothesis**: determines whether to support or reject the hypothesis.
   - [x] **Graphical Data Visualization**: illustrates some of the results graphically.
  
6. Conclusion
   - Summarize the results by given the company a *prospective financial return* based on the analysis' suggestions. 

## :mag_right: Becoming familiar

### Business problem
The questions answered on this analysis are:
- Which houses should Greener Houses buy and how much should the company pay for them?
- Once the house is acquired, when should it be sold and at what price?
- Should Greener Houses renovate a house to increase the sale price?

### Solution planning
The main steps taking to solve the business problem were as summarized below:
- Collecting and organizing data;
- Grouping data per region (zipcode);
- Finding the houses prices median for each region;
- Suggesting to buy the houses in good conditions that have prices lower than the median of its region.
- Grouping data per seasonality;
- Finding the new houses prices median within each set of region and seasonality;
- Updating the suggestions based on the set of conditions analyzed.

### 3 relevant insights
After carefully studying the dataset, some insights could be revealed. Three of them are listed below:
1. When analyzing *if houses overlooking the waterfront were about 30% more expensive than houses not overlooking the waterfront on average*, we found out that, actually, their prices are higher than **200%** comparing.

![image](https://github.com/quelcamara/ds-portfolio-insight-project-01/blob/main/plots/average-prices-for-houses-either-overlooking-or-not-the-waterfront.png)

2. While expecting that houses with basements would have a total area (square foot lot) 40% larger than houses without basements on average, we found out that, on the opposite, houses without basements have a total area larger than houses with this spare room. This difference was calculated on 18% on average.

![image](https://user-images.githubusercontent.com/73648823/114230229-40967380-994f-11eb-8796-67fae7e46832.png)

3. If we first thought that houses with 3 bathrooms could have a MoM positive growth within time, on the analysis we actually discovered that they don't seem to have a meaningful growth and that their prices variation were very *miscellaneous*.

![image](https://user-images.githubusercontent.com/73648823/114230160-28265900-994f-11eb-8433-68cfe5cc4a87.png)


### Financial results
As a result of this analysis, the company Greener Houses has about 11840 good deals on the construction market.

If the company chooses to invest only on the two more profitable regions out of the seventy available, it would still have 216 houses stated as good deals. This would represent a rate of 3 to 4 houses per month over the next 4 to 6 years, totalizing an average profit of U$234.344,38 per house and about U$700.000 to U$1.000.000 per month.

### Conclusion
With this analysis, Greener Houses is now capable of making its decisions based on the market opportunities, the financial returns, and also on the company revenue available to invest on these businesses. Moreover, the best time for selling and the profits for each deal will also be available for the company to evaluate prior to the decision-making.

It is then possible to say that the main goal of this analysis could be achieved.

## :hammer_and_wrench: Technologies
This project was built with the following technologies:
* [Python](https://www.python.org/downloads/) --version: 3.9.2
* [Jupyter Lab](https://jupyter.org/install) --version: 3.0.10
* [Pandas](https://pandas.pydata.org/) --version: 1.2.3
* [Numpy](https://numpy.org/) --version: 1.19.2
* [Matplotlib](https://matplotlib.org/) --version: 3.2.1
* [Seaborn](https://seaborn.pydata.org/) --version: 0.11.1

## :rocket: Setup
You have two ways to open this jupyter file: on your localhost or online.

If your only need is to see the notebook, there is no installation required, just jump into the [Executing online](#executing-online) topic and follow the directions.

However, if you want to edit or manipulate the code, it will be necessary to have some basic configurations done on your machine to execute the project. See the on the topic [Requirements](#requirements) below.

:bulb: You also won't be able to manipulate the file if you don't have your local server running the `Jupyter Lab`. For this, you can have a full explanation on the [Executing via cmd](#game_die-executing-via-cmd) step.

### Requirements
Before you get started, you will need to have [Python](https://www.python.org/downloads/) installed on your machine as well as the [Jupyter Notebook or Jupyter Lab](https://jupyter.org/install). There is no need to have any specific code editor or IDE if you wish to work on the code - you can do it directly on the notebooks.

Since it is not externally deployed, you will need to download the [ds-portfolio-insight-project-01](https://github.com/quelcamara/ds-portfolio-insight-project-01) project into your computer to be able to run it locally.

❗ But remember, if you only want to snoop into the code and have no interest on changing it, there is no need to trouble with this. You can also forget about the [Installation](#wrench-installation) and just go directly to the topic [Executing online](#globe_with_meridians-executing-online).

#### :wrench: Installation
If you have different versions of the technologies used to create this project, no need to panic! It won't be necessary to uninstall everything. You can always give it a try on running it on you machine with the current versions you already have and see if it works. If something goes wrong - because packages and functions are constantly being updated - you can easily create a virtual environment and then install only what you need.

You can follow the steps below if you need to create and configure a virtual environment. These are for Windows command-line, if you are a Linux or MacOS user, you will need to look for the likely commands. On the Command Prompt (cmd):

```shell
# Open the project directory (full path here)
$ cd C:\..\portfolio-insight-project

# Create the virtual environment (choosing python 3.9.2)
$ virtualenv venv --python=python3.9.2

# Access the virtual environment
$ venv\Scripts\activate.bat
```
After that, you will see a `(venv)` sign on the command-line indicating that you are now inside the virtual environment. It should look like this:
```shell
$ (venv) C:\..\portfolio-insight-project>_
```
Finally, you can install the technologies you need with whatever version you want inside your environment, and it won't affect at all any package you have on your operational system. Use the `pip install` for that:

> Just a friendly reminders here!<br/>
If you have installed <b>Anaconda</b> on your computer at any moment in your life, you probably already have all those packages available for you. Check for their versions and, if you have any troubles executing the Notebooks, create the virtual environment and install the packages using `conda` instead of `pip`.

```shell
$ pip install pandas==1.2.3
$ pip install numpy==1.19.2
$ pip install matplotlib==3.2.1
$ pip install seaborn==0.11.1
```
With these configurations, your machine is now ready to run and manipulate the project.

#### :globe_with_meridians: Executing online
To run the notebook online, you'll first need to download the [Greener_Houses.ipynb](https://github.com/quelcamara/ds-portfolio-insight-project-01/blob/main/Greener_Houses.ipynb) file on this repository.

Then, you can access a Jupyter Lab free and online server [here](https://jupyter.org/try). Scroll over the page and choose the JupyterLab option. It will redirect you to an online version of the tool that will allow you to open the file you have just downloaded.

Go to your local repository where the downloaded file is and then drag the .ipynb file into the left sidebar of the online tool. The field should be seen with a hashed border before you drop it. Wait a little bit while it is loaded and then just double click on the project once it is there under the sidebar options.

#### :game_die: Executing via cmd
To run the project and have access to the Notebooks:
```shell
# Go to the project directory (full path here)
$ cd C:\..\portfolio-insight-project

# Open the directory on the Jupyter Lab
$ jupyter lab
```
Just be patient here if your computer takes a little while without seeming to do a thing at all. It will process your inquisition and then open an external page on the web (your default browser) running the server on your localhost. You don't need to enter anything else on the command-line until this page is opened.

## :superhero: Author
<img src="https://avatars3.githubusercontent.com/u/73648823?s=460&u=81cc56a7c802bd21b265dfb0dadadccce01ec987&v=4" height="100" width="100">
Raquel Câmara Porto :maple_leaf:

<a href="https://www.linkedin.com/in/raquel-camara/"><img src="https://img.shields.io/badge/-Raquel-%230077B5?style=flat-square&logo=linkedin&logoColor=white"></a> <a href="mailto:raquelc.porto@outlook.com"><img src="https://img.shields.io/badge/-raquelc.porto@outlook.com-%230078D4?style=flat-square&logo=microsoft-outlook&logoColor=white"></a>
