---
title: Data Structure
layout: content
toc: true
---

<center>
<img src="/img/DataLake_Stage.png" width="80%"/>
</center>

* Table of Contents 
{:toc}
<br>

# DataLake Creation
The Colav data lake is all the raw data collected from the different sources and it is loaded in collections in a MongoDB.
The sources are handled by WOSPlus for Scielo, Scopus and Web of Science and in the future will be integrate with lens org.


# ETL
ETL ( Extract, Transform and Load) is a usual technique to create stages and dataware houses, In 
out case we dont need a data warehouse and we are server the data directly from the data stage.
The process is to take the data from the data lake and we are validation the papers with Google Scholar 
to create the Stage. For more detatils see [GSLookUp](GSLookUp) 


# Data Normalizacion Conventions
TODO 

# Stage 
Stage is the database after we read data from the Data Lake using GSLookUp and for the creation we need to apply
ETL techniques. After that we save the data in mongodb in the stage collection.
The Stage data will be served by PDBServer in a endpoint and this data is the official data to use in the indicators
and visualizations.
All the Colav software plugins will use the stage endpoint like official data input to do data processing.   

# EndPoints
All the endpoints are served using [PDBServer](PDBServer), every endpoint well need a query options and a apikey 
to access to the data.
