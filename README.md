✈️ Flight Price Alert System

This project is a Python-based flight deal alert system that monitors flight prices from a fixed origin city and notifies users when cheaper flights are found. It integrates multiple APIs to fetch destination data, search for flights, identify the cheapest available options, and send real-time notifications via WhatsApp.

🚀 Features

Fetches destination data from a Google Sheet

Automatically updates missing IATA airport codes

Searches for flights over the next 6 months

Identifies the cheapest available flight for each destination

Sends WhatsApp alerts when a lower-priced flight is found

Implements request throttling to avoid API rate limits

🛠️ Technologies Used

Python 🐍

Requests

DateTime & Time modules

Google Sheets API

Flight Search API (e.g., Tequila / Kiwi)

Twilio WhatsApp API

📂 Project Structure
flight-price-alert/
│
├── main.py
├── data_manager.py
├── flight_search.py
├── flight_data.py
├── notification_manager.py
└── README.md

⚙️ How It Works

Retrieves destination data from Google Sheets

Checks and fills missing IATA airport codes

Searches for flights from the origin city to each destination

Finds the cheapest available flight within the next 6 months

Compares prices with stored lowest prices

Sends a WhatsApp alert if a cheaper deal is found

🔑 Configuration

Update the following values before running the project:

ORIGIN_CITY_IATA = "LON"


Ensure API keys, tokens, and credentials are securely stored using environment variables (recommended).

▶️ How to Run
pip install -r requirements.txt
python main.py

📸 Sample Alert
Low price alert! Only £199 to fly from LON to PAR,
on 2024-03-12 until 2024-03-19.

🧠 Learning Outcomes

Working with multiple APIs

Automating price comparison logic

Handling date ranges dynamically

Modular Python project structure

Real-world notification systems

📌 Future Enhancements

Email notifications

Multiple origin cities

Scheduled execution (cron / cloud)

Improved error handling and logging
