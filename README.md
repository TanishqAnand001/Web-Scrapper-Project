# GitHub Topics Web Scraper

This project is a Python-based web scraper designed to extract information about various topics and their associated repositories from GitHub. It systematically navigates through the GitHub topics page, gathers details for each topic, and then proceeds to scrape the top repositories listed under each of them. The collected data includes topic titles, descriptions, repository names, authors, star counts, and repository URLs, which are then saved into a structured JSON file and can be viewed as a pandas DataFrame.

-----

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

  * **Python 3:** Ensure that you have Python 3 installed on your system.
  * **Git:** You will need Git to clone the repository.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/tanishqanand001/web-scrapper-project.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd web-scrapper-project
    ```
3.  **Create a virtual environment (recommended):**
    ```bash
    python3 -m venv venv
    venv\Scripts\activate
    ```
4.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

-----

## Usage

To run the web scraper and generate the `github_topics_repos.json` file, execute the Jupyter Notebook provided in the repository.

1.  **Start Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
2.  **Open the notebook:**
    Open the `Web Scrapper Project.ipynb` file in the Jupyter Notebook interface.
3.  **Run the cells:**
    Execute the cells in the notebook sequentially. The script will print the name of each topic as it is being scraped and will notify you upon completion.

The scraped data will be saved in the `github_topics_repos.json` file in the root directory of the project.

-----

## Project Structure

  * **`Web Scrapper Project.ipynb`**: The main Jupyter Notebook containing the Python code for the web scraper.
  * **`github_topics_repos.json`**: The output file where the scraped data is stored in JSON format.
  * **`requirements.txt`**: A list of the Python libraries required to run the project.

-----

## Built With

  * [requests](https://requests.readthedocs.io/en/latest/) - The elegant and simple HTTP library for Python, used to make requests to the GitHub website.
  * [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) - A Python library for pulling data out of HTML and XML files.
  * [pandas](https://pandas.pydata.org/docs/) - A powerful data manipulation and analysis library, used here to display the scraped data in a structured DataFrame.
  * [json](https://docs.python.org/3/library/json.html) - A lightweight data-interchange format, used for saving the scraped data.