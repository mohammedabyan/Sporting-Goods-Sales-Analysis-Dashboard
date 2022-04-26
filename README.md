<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mohammed-abyannash-400073194/)

<!-- PROJECT LOGO -->
<br />
<div align="center">

  <h2 align="center">Sporting Goods Store Analysis and Dashboard using SQL PBI</h3>

  <p align="center">
    Front-to-end process starting from data cleansing to creating a dashboard for Olympics Database
    <br /><br />
    <a href = https://www.dropbox.com/s/3sxwx52o3x8ozj7/olympic_games.bak?dl=0>Dataset</a>
  </p>
</div>

![image](https://user-images.githubusercontent.com/29911769/165216216-dcafcafd-0b47-48ad-9c7d-0d5db7ff868d.png)
![image](https://user-images.githubusercontent.com/29911769/165216319-110d3d18-d9cd-4e63-9c3c-b8c9b86d70f1.png)


<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#business-problem">Business Problem</a></li>
    <li><a href="#data-collection-and-table-structures">Data Collection and Table Structures</a></li>
    <li><a href="#olympic-games-analysis">Olympic Games Analysis</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>
<p align="right">(<a href="#top">back to top</a>)</p>

## Business Problem

The challenge for this data analyst project is outlined below. This has been used continuously to ensure that the right data has been selected, transformed and used in the data visualization which is meant to be passed on to the business users.

**"As a data analyst working at a news company you are asked to visualize data that will help stakeholders understand sales performance over time.**

**You also know that there is an interest in details about the category, products, and customers find anything interesting then don't hesitate to bring that in so if you also."**

<p align="right">(<a href="#top">back to top</a>)</p>


## Data Collection and Table Structures

The necessary data is first put into and SQL database and afterwards and transformed. Most of the tables were clean and ready to use but the budget table needed cleaning and formatting to make it machine-friendly

### Budget Table

![image](https://user-images.githubusercontent.com/29911769/165216603-f6829f32-04c2-47a7-9ce6-893eb586dcdc.png)
![image](https://user-images.githubusercontent.com/29911769/165216814-9aca5728-fc1d-4c15-a14c-6bc6c1797b1b.png)

The final model is as shows
![image](https://user-images.githubusercontent.com/29911769/165216319-110d3d18-d9cd-4e63-9c3c-b8c9b86d70f1.png)
The strucutre of the model allows for cross-referncing and slicing data between tables efficiently by using the Sales as a fact table supported by look-up tables.

## Calculations

The following calculations were created in the Power BI reports using DAX (Data Analysis Expression). To lessen the extent of coding, the re-use of measures (measure branching) was emphasized:

Sales:
```
Sales = SUM(Sales[SalesAmount])
```
Total Sales:
```
Total Sales = SUM(Sales[SalesAmount]) + SUM(Sales[TaxAmt])
```
Budget:
```
Budget = SUM(Budget[Budget Amount])
```
Variance:
```
Variance = [Sales] - [Budget]
```
Variance %
```
Variance% = DIVIDE([Variance],[Budget])
```
<p align="right">(<a href="#top">back to top</a>)</p>

## Olympic Games Analysis

The final dashboard features all the necessary visualizations required by the stakeholders. We are able to view the data to quite a granular level by using the drill down feature. Customer spending and top products can also be found on the lefthand side of table which can be used to narrow down the data shown by clicking on the values.

[here](https://github.com/mohammedabyan/Olympic-Games-Data-Analysis-SQL-PBI/raw/main/Olympic%20Games%20Dashboard.pbix).

![image](https://user-images.githubusercontent.com/29911769/165217243-10b0eb07-0dc8-46d1-8d4d-cfd067c4fb37.png)

<p align="right">(<a href="#top">back to top</a>)</p>


## Contact

Mohammed Abyannash - mohammedabyan22@gmail.com

<p align="right">(<a href="#top">back to top</a>)</p>


