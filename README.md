<p align="center">
    <img src="./images/icons/python.PNG" alt="Python programming language logo." style="float: left;" width="40%">
    <img src="./images/icons/1024px-Scikit_learn_logo_small.svg.png" alt="Scikit Learn logo." style="float: right;" width="40%">
</p>

# Information Retrieval for Fault Localization Using LSI (Latent Semantic Indexing) and Other Methods

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Launch](#launch)
- [Screenshots](#screenshots)
- [Contributors](#contributors)

## Introduction
There are a number of approaches used for Fault Localization in potential bug files that use Information Retrieval (IR) methods. Common techniques are the BugLocator IR methods that utilize a ranking system based on direct and indirect linking of potential source file fixes. A well known technique such as BugLocator would be a relevant benchmark IR using Latent Semantic Indexing (LSI). By comparing metrics using two methods developed using BugLocator we can compare new IR methods using LSI to notice performance based on the accuracy and ranking of correct files. The first approach will be broken into two methods (methods 1 and 2) to facilitate a benchmark for the full implementation of BugLocator and LSI. The observations show a significant improvement from the full implementation due combining multiple approaches to ranking. Compared to single approaches multiple methods of ranking are leveraged for performance boosts.

Overall there are three methods that were implemented and evaluated:
- Method 1: Simplified BugLocator
- Method 2: Full BugLocator
- Method 3: Latent Semantic Indexing (LSI) with Singular Value Decomposition (SVD)

The pre-processing code up to the Markdown heading "More Pre-processing (Team 7)" in the Jupyter notebook was provided by a course instructor.

## Features
- Pre-processes metadata of answer to questions on Stack Overflow.
- Ranks source files (query results) related to a bug report (query) to find the location of bugs related to the bug report.
- NumPy style documentation for maintainability and clarity of application.

## Launch
### Setup
To run application, first install [Jupyter Lab](https://jupyterlab.readthedocs.io/en/stable/getting_started/installation.html), then open a new console and enter:
```
jupyter lab
```
This will open a jupyter lab tab in your default browser, in which you can run the application.

## Screenshots
### MRR Results (Mean Reciprocal Rank)
<img 
    src="images/results/MRR (Mean Reciprocal Rank) vs. Package.png" 
    alt="MRR (Mean Reciprocal Rank) vs. Package.">

<img 
    src="images/results/MRR Difference (method 2 - method 1) vs. Package.png" 
    alt="MRR Difference (method 2 - method 1) vs. Package.">

<img 
    src="images/results/MRR Difference (method 3 - method 1) vs. Package.png" 
    alt="MRR Difference (method 3 - method 1) vs. Package">

### MAP Results (Mean Average Precision)
<img 
    src="images/results/MAP (Mean Average Precision) vs. Package.png" 
    alt="MAP (Mean Average Precision) vs. Package.">

<img 
    src="images/results/MAP (Mean Average Precision) Difference (method 2 - method 1) vs. Package.png" 
    alt="MAP (Mean Average Precision) Difference (method 2 - method 1) vs. Package.">

<img 
    src="images/results/MAP (Mean Average Precision) Difference (method 3 - method 1) vs. Package.png" 
    alt="MAP (Mean Average Precision) Difference (method 3 - method 1) vs. Package">

Overall, method 2 shows the best performance.

## Technologies
- [Python version 3.8.2](https://www.python.org/downloads/release/python-382/)
- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [scikit-learn](https://scikit-learn.org/stable/)

## Contributors
<table>
    <thead>
        <tr>
            <th align="center">
                <a href="https://github.com/NikelausM">
                    <img alt="NikelausM" src="https://avatars3.githubusercontent.com/u/51514472?s=460&u=0e68a59a1bed0101bf500753790048630779cc9b&v=4" 
                         width="100" style="max-width:100%;">
                </a>
            </th>
            <th align="center">
                <a href="https://github.com/ConnorBritton">
                    <img alt="ConnorBritton" src="https://avatars2.githubusercontent.com/u/28262511?s=460&v=4" 
                         width="100" style="max-width:100%;">
                </a>
            </th>
            <th align="center">
                <a href="https://www.linkedin.com/in/philip-rea-40a524158/">
                    <img alt="Philip Rea" src="https://media-exp1.licdn.com/dms/image/C5603AQFB_H106kCYDg/profile-displayphoto-shrink_400_400/0/1581393138166?e=1614211200&v=beta&t=r2uWJ0v-CclsgHV1rGWNQ1UhFF6Z9c64XlYb2Wcww7c" 
                         width="100" style="max-width:100%;">
                </a>
            </th>
            <th align="center">
                <a href="">
                    <img alt="Joseph Park" src="" 
                         width="100" style="max-width:100%;">
                </a>
            </th>
        </tr>
    </thead>
<tbody>
<tr>
    <td align="center">
        <a href="https://github.com/NikelausM">Nicolas Mora</a>
    </td>
    <td align="center">
        <a href="https://github.com/ConnorBritton">Connor Britton</a>
    </td>
    <td align="center">
        <a href="https://www.linkedin.com/in/philip-rea-40a524158/">Philip Rea</a>
    </td>
    <td align="center">
        <a href="">Joseph Park</a>
    </td>
</tr>
</tbody>
</table>
