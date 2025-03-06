# IVOS-AI Web Application For Clinician Evaluation Study

## Overview
This is a Django-based web application with JavaScript frontend functionality. This repository contains the code, web app and data for the study presented in the paper "The impact of artificial intelligence-driven decision support on uncertain antimicrobial prescribing: a randomized multi-method study" (currently undergoing peer review).

If you use this code please cite this code repository and our associated publication.

### ** Notes **
- cdss/ is the main Django project directory and contains global settings and configurations.
- patients/ is a Django app handling patient-related models and views.
- Analysis of the results is conducted inside the cdss/analysis/ folder.
- Static assets (e.g., images and patient data) are in the images/, pdf/ and csv/ directories.
- The node_modules/ directory contains front end dependicies.
- The codebook and python code used for analysis of the interviews are contained within interview_materials/

## **Installation Instructions**

### **1. Prerequisites**
Ensure you have the following installed on your system:
- [Anaconda/Miniconda](https://docs.conda.io/en/latest/miniconda.html)
- [Python 3](https://www.python.org/downloads/)
- [Node.js](https://nodejs.org/)

### **2. Setting up the Environment**
1. Open a terminal and navigate to the project directory:

   	cd path/to/project

2. Create and activate the Conda environment from environment.yml:

	conda env create -f environment.yml
	conda activate cdss

Alternatively you can manually install dependencies:

	conda create --name cdss python=3.10.13
	conda activate cdss
	pip install -r requirements.txt

3. Install Node.js for frontend functionality:

	npm install

This project was developed using **Python 3.10.13**. Other versions (e.g., 3.9, 3.11) may work, but they have not been tested.

### **3. Running and accessing the Web Application**

Run the following command to start the server and reset the database: python runserver_plus_resetdb.py

Once the server is running, open your browser and go to: http://127.0.0.1:8000/

Login combinations include:
ID: demo, Archetype: a
ID: 50, Archetype: a
ID: 49, Archetype: b


