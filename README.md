# Website Summarizer

This project extracts and summarizes the content of a given website using OpenAI's API. The summary is generated in markdown format, ignoring navigation-related text and recognizing the language used on the webpage.

## Features
- Fetches website content and extracts relevant text
- Generates a short summary in markdown format
- Recognizes the website's language and responds in the same language
- Ignores navigation-related text

## Prerequisites
- Python 3.x
- `pip` installed
- OpenAI API key
- `.env` file for environment variables

## Installation

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd <repository-name>
   ```

2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```

3. Create a `.env` file in the project root and add your OpenAI API key:
   ```ini
   OPENAI_API_KEY=your-openai-api-key
   ```

## Usage

Run the script with a website URL to get a summary:
```sh
python script.py
```

### Example
```python
from summarize import display_summary

display_summary("https://example.com")
```

## Configuration
- Modify `system_prompt` in `summarize.py` to fine-tune the assistant's behavior.
- The script currently uses `gpt-4o-mini`. You can change this in the `summarize` function.

## Dependencies
- `openai`
- `python-dotenv`
- `requests` (if needed for fetching website content)

## License
This project is licensed under the MIT License.

