# Markdown to Google Docs Converter

A Python script that runs in Google Colab and converts markdown-formatted meeting notes into a well-formatted Google Doc using the Google Docs API.

## Features

- Converts markdown headings to Google Docs styles (H1, H2, H3)
- Maintains nested bullet points with proper indentation
- Handles checkboxes with custom formatting
- Highlights @mentions in bold red
- Includes distinct footer styling
- Error handling and detailed logging
- Easy to use in Google Colab environment

## Prerequisites

- Google Account
- Access to Google Colab
- Google Drive API access

## Setup Instructions

1. Clone this repository:
```bash
git clone https://github.com/sharan-sripada/markdown_2_gdocs.git
```

2. Open [Google Colab](https://colab.research.google.com)

3. Upload the `markdown_2_gdocs.ipynb` notebook to Colab:
   - Click File → Upload notebook
   - Select the notebook from your cloned repository

## Required Dependencies

The notebook will automatically install these dependencies:
```python
!pip install google-auth-oauthlib google-auth-httplib2 google-api-python-client
```

## How to Run in Colab

1. Open the uploaded notebook in Colab
2. Run all cells (Runtime → Run all)
3. When prompted, authenticate with your Google account
4. The script will create a new Google Doc and provide you with the document ID
5. Check your Google Drive for the newly created document

## File Structure

```
markdown_2_gdocs/
├── README.md
├── markdown_to_gdocs.ipynb
```

## Example Usage

The notebook includes a sample meeting notes template. To use your own markdown:

1. Replace the `markdown_content` variable with your own markdown text
2. Update the `title` variable if desired
3. Run the cell

## Error Handling

The script includes comprehensive error handling for:
- Authentication failures
- API errors
- Invalid formatting requests
- Missing or malformed content



## Acknowledgments

- Google Docs API Documentation
- Python-Markdown library
- Google Colab team

