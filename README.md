# OPEC Ridgeline [Visualization](https://xuanx1.github.io/opecRidge/opec_ridgeline_plot.html)

A data visualization project that analyzes and visualizes OPEC (Organization of the Petroleum Exporting Countries) petroleum production data from 2014 to 2024 using interactive ridgeline plots.

## [Preview](https://xuanx1.github.io/opecRidge/opec_ridgeline_plot.html)
![Screenshot 2025-08-23 233139](https://github.com/user-attachments/assets/4cc318b6-407e-4eee-bc26-dc0ce4d7d869)

## Project Overview

This project extracts petroleum production data from OPEC Annual Statistical Bulletins (PDF format) and creates an interactive ridgeline plot to visualize production trends across OPEC member countries over the past decade.

### Key Features

- **Data Extraction**: Automated extraction from OPEC PDF reports (2014-2024)
- **Interactive Visualization**: D3.js-powered ridgeline plot showing production distributions
- **Clean Data Pipeline**: Processed and cleaned datasets for analysis
- **Comprehensive Coverage**: All OPEC member countries included

## Data Sources

The project uses official OPEC Annual Statistical Bulletins from 2014-2025, covering production data for:

- Algeria
- Angola
- Congo
- Ecuador
- Equatorial Guinea
- Gabon
- Indonesia
- Iraq
- Kuwait
- Libya
- Nigeria
- Qatar
- Saudi Arabia
- United Arab Emirates
- Venezuela

## Project Structure

```
├── README.md                           # Project documentation
├── opec_ridgeline_plot.html           # Interactive visualization
├── merged_opec_2014_2024_opec.csv     # Final merged dataset
└── processing/                        # Data processing files
    ├── extract_opec_pdf.ipynb         # PDF extraction notebook
    ├── *_cleaned_opec_only.csv        # Cleaned OPEC-only datasets
    ├── *.pdf                          # Source OPEC bulletins
    └── *.csv                          # Raw extracted data
```

## Getting Started

### Prerequisites

- Web browser (for viewing the visualization)
- Python 3.x (for data processing)
- Required Python packages: `pandas`, `pdfplumber`

### Viewing the Visualization

Simply open `opec_ridgeline_plot.html` in your web browser to interact with the visualization.

### Data Processing

1. **PDF Extraction**: Use `processing/extract_opec_pdf.ipynb` to extract data from PDF files
2. **Data Cleaning**: The notebook processes and cleans the extracted data
3. **Merging**: Combines data from different years into the final dataset

## Technical Details

- **Visualization**: Built with D3.js v7
- **Data Format**: CSV with countries as rows and years as columns
- **Processing**: Jupyter notebook for PDF text extraction and data cleaning
- **Styling**: Custom CSS for professional presentation

## Data Notes

- Production values are in thousands of barrels per day
- Some data points may contain missing values (represented as "1" in original data)
- Data spans 2014-2024 covering the most recent decade of OPEC production

## Usage

The interactive ridgeline plot allows you to:
- Explore production trends for each OPEC member country
- Compare production levels across different years
- Identify patterns and changes in petroleum production

## Contributing

Feel free to submit issues or pull requests to improve the visualization or data processing pipeline.

## License

This project is for educational and research purposes. Data is sourced from official OPEC publications.
