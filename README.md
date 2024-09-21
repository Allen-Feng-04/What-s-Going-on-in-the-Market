# What's Going on in the Market Today?

## About the dataset
The program will generate a dataset that includes links to all the current day's news and public company press releases, such as shareholder meetings, lawsuits, and board announcements. It will also provide information on how the related stocks are performing.

##Sources used

- **Stockhouse.com**: A static website that posts recent stock news and board announcements. As scraping on most of its pages is allowed, our program will scrap stock press releases from this website.
- **https://twelvedata.com**: This API will then provide the relevant stock movement information for the day.


## Why do people need it
This dataset provides a quick and comprehensive snapshot of how news and press releases are influencing stock movements in real time. By consolidating major announcements—such as shareholder meetings, lawsuits, or board decisions—and relevant stock performance, professionals can easily identify key factors driving market trends. Whether it's a stock surging due to a product release or falling due to legal concerns, users will be able to assess the situation at a glance, making it an invaluable tool for timely decision-making. The live nature of the dataset ensures that it's always up-to-date, making it especially useful for traders, analysts, and investors who need to stay on top of market-moving events. 

## How to Run

**Requirements**:

Acquire your own API key from https://twelvedata.com

1. **Clone the Repository**

   To get started, first clone the repository to your local machine:

   ```bash
   git clone https://github.com/Allen-Feng-04/What-s-Going-on-in-the-Market
   cd What-s-Going-on-in-the-Market
   ```

2. **Install Dependencies**

   Create a virtual environment and install the required packages:

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows, use `env\Scripts\activate`
   pip install -r requirements.txt
   ```

3. **Run the Script**

   Add your own API key to the your_API_key variable, and change the date argument in the get_and_write_all_stock_movements function to yesterday's date or any past date
   (Both the function and variable are in the last two lines of main.py)

   ```bash
   python main.py
   ```
   The script will then produce the dataset. 
