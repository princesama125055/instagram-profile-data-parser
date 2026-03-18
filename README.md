# Data Parsing and Analysis Project

This project is built using Core Python and Jupyter Notebook.  
It parses raw Instagram-style profile data from a text file, converts it into structured JSON format, and performs basic data analysis on the extracted records.

## Project Overview

The input data contains unstructured social media profile information such as:

- username
- number of posts
- followers
- following
- profile name
- page type
- bio

The program reads raw text data, separates each profile, extracts useful fields, handles values like `K` and `M` in follower counts, and stores the cleaned data in dictionary/JSON format for analysis. 

## Features

- Read raw text data from input file
- Split and parse multiple profile records
- Extract structured fields from unstructured text
- Convert follower/following counts like `22.4K` and `38K` into numeric values
- Handle missing fields safely
- Store final cleaned data in JSON format
- Perform basic analysis such as:
  - maximum posts
  - follower comparisons
  - profile-level insights 

## Tech Stack

- Python
- Jupyter Notebook
- JSON
- File Handling
- Core Python Data Structures

## Project Files

- `coders-of-bangalore_by_me.ipynb` — main Jupyter Notebook containing the parser and analysis code
- `initialdata.txt` — raw input dataset
- `finaldata.txt` — extended/cleaned input dataset
- `data.json` — structured JSON output generated from parsed records 

## How It Works

1. Read raw profile data from a text file
2. Split the data into separate profile chunks
3. Parse each chunk line by line
4. Extract fields like username, posts, followers, following, name, type of page, and bio
5. Convert text-based numeric values into integers
6. Save the cleaned data into JSON format
7. Run analysis on the parsed dataset

## Sample Parsed Output

```python
{
    "username": "techie_koramangala",
    "posts": 420,
    "followers": 9800,
    "following": 310,
    "name": "Arjun M.",
    "type_of_page": "Software Engineer",
    "bio": "💻 Full-stack @ SaaS startup\n☕ Working from cafes in Koramangala\ngithub.com/arjunmakes"
}
