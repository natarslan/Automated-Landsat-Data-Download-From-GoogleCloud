# Automated Landsat Data Download From GoogleCloud
A script to bulk download public Landsat satellite imagery from Google Cloud

## The original script 
Script to download data from Amazon Web Services can be found [here](http://geologyandpython.com/get-landsat-8.html)  

## Why a different script for Google Cloud?
Google Cloud holds more satellite imagery (at least for the time being). Direct implementation of above script didn't work to access and bulk download the Google Cloud data. The changes can be seen in step 10, 11 & 12 where the dataframe is edited to access to the correct Google URL.

## Important parts to keep an eye on when you use this code
1. You can use [geojson.io](http://geojson.io/#map=2/20.0/0.0) to get your study area coordinates
2. Change the scene filters according to your need (cloud cover and date for instance)
3. Satellite collections might have different number of bands. Change the range in download step accordingly. For example use "for x in range(1, 9):" for Landsat-8 bands

## Issues
* Current version doesnt download BQA band and metadata

