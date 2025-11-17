# Globussoft
Globussoft Assessment – Python Projects

This repository includes two independent Python projects developed for the Globussoft assessment. Each project contains its own code, dependencies, and instructions for running.

**Project 1: Amazon Laptop Data Scraper**

A Python script that collects laptop information from Amazon.in and saves it into a CSV file for analysis.

What It Does

Downloads product images

Retrieves product names

Captures ratings (if available)

Extracts price information

Marks products as Ad (sponsored) or Organic

How to Run

Make sure you have Python 3.x installed.

Install required packages:

pip install -r requirements.txt


Run the scraper:

python amazon_scraper.py


A CSV file will be generated automatically with a timestamped filename.

Folder Structure
Task1/
├─ amazon_scraper.py       # Main script for scraping
├─ amazon_laptops_*.csv   # Sample CSV output
└─  requirements.txt        # Python packages needed

**Project 2: Face Authentication API (FastAPI)**

A Python-based API service using FastAPI to check if two face images belong to the same person using deep learning embeddings.

Key Features

Accepts two face images

Detects faces in both images

Returns:

Verification result: Same or Different person

Similarity score

Bounding boxes of detected faces

How to Run

Ensure Python 3.x is installed.

Install dependencies:

pip install -r requirements.txt


Start the FastAPI server:

cd Task2
uvicorn app:app --reload


Open your browser at:

http://127.0.0.1:8000/docs


You can test the API using the interactive Swagger interface.

Folder Structure
Task2/
├─ app.py                # FastAPI application
├─ test_images/          # Sample images for testing
│  ├─ img1.jpg
│  ├─ img2.jpg
│  └─ img3.jpg
├─ requirements.txt      # Python dependencies
└─ README.md             # Instructions
