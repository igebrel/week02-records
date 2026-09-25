# Week 02 - TVMaze Records Processing

## Overview

This project downloads TV show records from the TVMaze API and processes the returned data using Python. The program organizes the records and creates an aggregated summary in JSON format.

## Files

- `records.py` - Downloads and processes TV show records.
- `summary.json` - Contains the generated summary results.
- `requirements.txt` - Lists the Python package required by the project.
- `.gitignore` - Specifies files and folders that Git should ignore.

## Requirements

- Python 3.11 or later
- requests

## Installation

Create and activate a virtual environment, then install the required package:

```bash
pip install -r requirements.txt

## How to Run

Run the program from the terminal:

```bash
python records.py
```

## Output

The program prints the number of processed TV show records and creates `summary.json` containing the aggregated results.

## Acknowledgement

I used ChatGPT for guidance when I had questions about setting up the project, using Git, and checking my work. I reviewed the code and tested the program before completing the project.

## Data Quirks

The TVMaze API may contain missing or incomplete values for some TV shows. For example, some records may not include a language, genre, or rating. The program checks these values before processing the records so that missing data does not cause the program to fail.

## Design Choices

I used different Python collections to organize the data. I used a dictionary to group the TV shows by genre, a set to keep the unique languages, and a list to store the records. I also used a comprehension when processing the data. I chose these collections because they made it easier for me to organize and summarize the TV show records.

## Known Limitations

The program depends on the TVMaze API, so it needs an internet connection to download the records. If the API is unavailable, the program cannot get the data. The results also depend on the information provided by the TVMaze API.
