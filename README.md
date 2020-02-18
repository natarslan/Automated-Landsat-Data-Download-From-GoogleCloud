# Automated Landsat Data Download From GoogleCloud
A script to bulk download public Landsat satellite imagery from Google Cloud

## The original script 
Script to download data from Amazon Web Services can be found [here](http://geologyandpython.com/get-landsat-8.html)  

## Why a different script for Google Cloud?
Direct implementation of above script didn't work to access and bulk download the Google Cloud data. The changes can be seen in step 10, 11 & 12 where the dataframe is edited to access to the correct Google URL.

## Issues
* Current version doesnt download BQA band and meta data
