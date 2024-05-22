# GitHub Search API Script

This Python script allows you to search for repositories on GitHub using the GitHub Search API. It retrieves information about the repositories related to the specified search query and stores the data in a CSV file.

## Features

- Search for repositories based on a query (e.g., "machine+learning").
- Retrieve repository details such as name, description, stars, watchers, forks, open issues, primary language, license, and relevance score.
- Calculate the percentage of languages used in each repository.
- Save the retrieved data in a CSV file with the filename based on the search query.

## Prerequisites

- Python 3.x
- `requests` library (install with `pip install requests`)

## Usage

1. Clone the repository or copy the script to your local machine.
2. Open the script in a text editor and replace `"access_token_here"` with your GitHub personal access token. You can create a new token by following the instructions at [https://github.com/settings/tokens](https://github.com/settings/tokens).
3. Save the changes to the script.
4. Run the script using the command `python script_name.py`.
5. When prompted, enter the search query you want to use (e.g., "machine+learning").
6. The script will search for repositories related to the query and save the results in a CSV file with the same name as the query (e.g., "machine+learning.csv").

## Notes

- The script retrieves up to 1000 results (the maximum allowed by the GitHub Search API).
- If you encounter rate-limiting issues with the GitHub API, you can uncomment the `time.sleep(10)` line to introduce a delay between requests.
- The script prints the retrieved repository information to the console for reference.

## License

This project is licensed under the [MIT License](LICENSE).
