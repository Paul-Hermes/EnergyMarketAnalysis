# Energy Market Analysis Project - by Paul J. Hermes

This is a project exploring the european energy market.

## Prerequisites

  - conda (I used version 26.1.1)
  - API Key for the ENTSO-E Transparency Platform
  - API Key for the Copernicus Climate Data Store

## Setup

After acquiring the needed prerequisites execute the following commands in your terminal:
    
    conda env create -f environment.lock.yml
    conda activate eu-energy-market
    cp .env.example .env

At this point open your favourite editor and place your own API keys in the dedicated fields of the .env file.
Then run:
    
    jupyter lab

### (Updating the Environment)

In case you want to use more current versions of the here used packages, you can perform the following commands to update the environment.
It is possible this makes the packages not work together anymore. 
If you use the setup I descibed above you will be using _exactly_ what I am using which should work without bigger problems.
ONLY PERFORM IF YOU KNOW WHAT YOU ARE DOING:

    conda env update -f environment.yml --prune
    conda env export --no-builds > environment.lock.yml

## Contents

    01_acquisition.ipynb - How to get the data I will be using

## Notes

All data used stems from:

 - ENTSO-E, "ENTSO-E Transparency Platform", 2026. [Online]. Available: https://transparency.entsoe.eu/. [Accessed: 10.09.2026].
 - H. Hersbach et al., "ERA5 hourly data on single levels from 1940 to present",
    Copernicus Climate Change Service (C3S) Climate Data Store (CDS), 2018.
    [Online]. Available: https://doi.org/10.24381/cds.adbb2d47.
    [Accessed: 13.09.2026].