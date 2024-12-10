<img width=90 src="https://www.ptse.nl/ptse-logo.png" align="right">

# Introduction
<details markdown='1'>
<summary>Polarion SQL webinar</summary>

- Welcome: Organised by **P**rofessional in **T**ools for **S**ystems **E**ngineering (PTSE) 
  - owner Henk Broeze (INCOSE ESEP & OMG UML/SysML certified) 
  - broeze@ptse.nl
- Objective:  Basics SQL & **How** and **Where** toe use SQL in Polarion queries, 
- Logistics: Recording / share material?
  - Duration: 45 min followed by Q&A on posted questions in Teams
 </details>
 
<img style="float:right;" width=90 src="https://www.ptse.nl/ptse-logo.png" align="right">
  
# 1. SQLbasics
<details markdown='1'>
<summary>Standardized query and data manipulation language for Reltional databases. </summary>

## Relational database
## SQL Syntax
   SELECT \<clause\>  
   FROM \<tables\>  
   WHERE \<conditions\>  
   
## Sample database
 
 ```mermaid
 classDiagram
 class countries {
 continent
country
}
 class codes {
 code
country
}
codes-->countries
```

## Sample Queries
|need|qiery|
|----|----|
|Filter on columns|All continemts in countries|SELECT continent FROM countries|
|Filter on special  olumn value|All countries in Europe|SELCT country <br/> FROM countries <br/>WHERE continent = 'Europe'|
|Combine tables|All codes from Europe|SELECT code<br/> FROM countries, codes <br/> WHERE  countries.country =  codes.country|

</details>

<img style="float:right;" width=90 src="https://www.ptse.nl/ptse-logo.png" align="right">

# 2. Intro SQL in Polarion
<details markdown='1'><summary>In Polarion the basic query technology is Lucent but can be extendedor replaced by SQL queries. </summary>

## Polarion database model

## Polarion tables subset

## Apply basic SQL queries to Polarion

## Polarion Lucene vs SQL

</details>

<img style="float:right;" width=90 src="https://www.ptse.nl/ptse-logo.png" align="right">


# Where can SQL be used in Polarion
<details markdown='1'><summary>Qjerying in Polarion  an be done at multiple locations</summary>
- Tracker, combined with Lucene (hint: SQL:(....))
- Widgets
- API:
	- Velocitiy scripting, queryWorkItems, searchInstances
	- Javascript (out of scope)
	- Rest API (out of scope)
-  Postgress database, the Polarion index database
    psql -U polarion -p 5433. 
</details>
<img  width=90 src="https://www.ptse.nl/ptse-logo.png" align="right">

# 4. Advanced funtions
 <details markdown='1'><summary>SQL has an extended set for making sopnisticated queries</summary>
## (P)SQL functions

## Frequently used functions
 |function|Meaning|example|
 |----|----|----|
 |COUNT|number of|SELECT COUNT(*)</br>FROM countries|
 |IN|value in a set|SELECT *</BR>FROM countries</br>WHERE continent IN ("Europe", 'Asia")
  
</details>


# 5. Applying math logic
<details markdown='1'><summary>Mathematic logic rulesapply to sopnisticated comditions</summary>
</details>

# 6. Combining SQL Queries
<details markdown='1'><summary>Mathematic logic rulesapply to sopnisticated comditions</summary>
</details>
 


# Conclusions
<details markdown='1'><summary>Take away and next webinar</summary>
- Powerfull and fast way for sophicated queries
- No debug and no sytax error messages in Polarion

## Next webinar candidates:
- Generate UML models from Polarion project configurations
- Query Polarion with Python pandas, Rest API based
- </details>

