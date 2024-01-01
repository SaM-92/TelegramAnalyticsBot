# Time Series Data Analysis Telegram Bot

## Overview

This Telegram bot is designed to automate the processing and analysis of time series data. It manages missing values, resamples data to an hourly resolution, and provides basic statistical analysis. The bot is especially beneficial for users engaged with time series datasets, particularly the ENTSO-E dataset.

## About ENTSO-E

In previous work [energy-data-entsoe](https://github.com/SaM-92/energy-data-entsoe/tree/main), the ENTSO-E Data Analysis Tool was developed as an interactive web application to simplify the analysis of [European Network of Transmission System Operators for Electricity (ENTSO-E)](https://transparency.entsoe.eu/) power system data. This tool was created to assist in efficiently handling, visualising, and analysing electricity market and grid data across Europe.

Building on this, a Telegram bot demo version has been crafted to explore a different approach. This version is designed for users who prefer interacting through Telegram rather than a web interface, offering a convenient and user-centric experience for data analysis on the go.



## Features

- **Data Upload Handling**: Users can upload CSV files directly to the bot.
- **Column Selection**: After uploading data, users can select a specific time column for easing the analysis.
- **Data Processing**: The bot interpolates missing values and resamples data to an hourly resolution.
- **Statistical Analysis**: It provides basic statistics of the processed data.
- **File Download**: Users can download the processed data as a CSV file.

## Installation

1. Clone the repository:

``` git clone https://github.com/SaM-92/TimeSeriesDataAnalysisTelegramBot.git ```

2. Install the required dependencies:
``` pip install -r requirements.txt ```


## Usage

Before using the Telegram bot, make sure you have completed the installation steps. Then, follow these instructions to run the bot and interact with it on Telegram:

### Setting Up the Bot

1. **Obtain a Telegram Token**:
   - First, you need a Telegram bot token. Create a new bot on Telegram by chatting with [BotFather](https://t.me/botfather).
   - Follow BotFather's instructions to create a new bot. Once created, BotFather will provide you with a token.
   - Save this token; you will need it to run your bot.

2. **Configure the Bot**:
   - Set the token as an environment variable or directly in your `main.py` script (not recommended for security reasons).

3. **Run the Bot**:
   - Execute the `main.py` file to start your bot. In your terminal or command prompt, navigate to the bot's directory and run:
     ```
     python main.py
     ```

### Interacting with the Bot on Telegram

- Start the bot using the `/start` command.
- Upload a time series data file in CSV format.
- Select the appropriate time column when prompted.
- The bot processes the data and sends back a file with the results.

## Commands

- `/start` - Begin the interaction and upload data.
- `/help` - Get instructions on how to use the bot.
- `/about` - Information about the bot and its capabilities.

## Development

This bot is built using Python and the `python-telegram-bot` library. It leverages Pandas for data processing and analysis.

## Contributing

Contributions to the bot are welcome. Please feel free to fork the repository, make improvements, and submit pull requests.

## License

This repos is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).