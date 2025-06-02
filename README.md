# Supreme Court Technology Analysis 
Analysis of technology-related discussions in US Supreme Court cases (October 2023 - April 2024).
Overview
This project scrapes Supreme Court oral argument transcripts and written opinions to identify cases mentioning technology-related terms.

## Data Pipeline:

Scraped oral argument metadata from transcript listings
Scraped slip opinion metadata from court decisions
Merged datasets on docket numbers to create comprehensive case database
Downloaded and analyzed full text documents for keyword frequency

Built final dataset of 58 cases with metadata, clickable transcript links, and opinion links.

## Tech Stack

Python - pandas, requests, BeautifulSoup, matplotlib
Data Sources - supremecourt.gov transcripts and slip opinions
Analysis - Keyword frequency detection and visualization

## Key Results

58 cases analyzed from 2023-2024 term
7 cases mentioned "technology" in oral arguments
2 cases mentioned "misinformation" (Murthy v. Missouri, Moody v. NetChoice)
Generated pie chart visualization of technology mention distribution

## Usage

bash# Install dependencies
pip install pandas requests beautifulsoup4 matplotlib jupyter

## Run analysis
jupyter notebook supreme_court_analysis.ipynb
Project Structure
├── supreme_court_analysis.ipynb    # Main analysis notebook
├── data/
│   ├── oral_argument_transcripts.csv
│   └── court_docs/                 # Downloaded PDFs
└── visualizations/                 # Generated charts

## Future Improvements

Add geographical data of lower courts
Enhanced contextual analysis: Extract full sentences containing keywords, identify document sections with mentions, and determine context (positive/negative, procedural vs. substantive)
Implement NLP with spaCy for semantic understanding beyond simple keyword matching
Create interactive visualizations
Expand keyword search capabilities
