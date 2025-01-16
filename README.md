# Weather Reminder Project

This project consists of two Python scripts that provide weather updates and reminders via email and desktop notifications. The scripts use web scraping to gather weather data and send timely notifications or by email to users.

## Features
- **Weather Reminder on Email**: Sends daily weather updates to users' email addresses with a reminder to carry an umbrella if necessary.
- **Weather Notification**: Displays weather updates as desktop notifications using the `win10toast` library.
- **User Details Management**: User details are stored in a JSON file for easy management.

## Project Structure

```
├── WeatherReminderEmail.py
├── WeatherNotification.py
├── User_details.json
├── sender_details.txt
└── README.md
```

## Files

### 1. `WeatherReminderEmail.py`
This script sends weather updates via email. It scrapes weather information from Google and sends an email with the weather details to the users listed in `User_details.json`.

#### Key Libraries Used
- `BeautifulSoup`: For web scraping.
- `smtplib`: For sending emails.
- `schedule`: For scheduling daily email reminders.
- `pandas` and `dataframe_image`: For handling and formatting weather data.

#### Usage
1. Add your email and password to `sender_details.txt`.
2. Update `User_details.json` with the user information.
3. Run the script to send daily weather updates.

### 2. `WeatherNotification.py`
This script provides weather updates as desktop notifications. It also scrapes weather information from Google and displays it using the `win10toast` library.

#### Key Libraries Used
- `BeautifulSoup`: For web scraping.
- `schedule`: For scheduling notifications.
- `win10toast`: For displaying desktop notifications.

#### Usage
1. Set the desired city name in the script.
2. Run the script to receive periodic weather updates as desktop notifications.

### 3. `User_details.json`
This JSON file contains user information such as names and email addresses. It is used by `WeatherReminderEmail.py` to send weather updates.

### 4. `sender_details.txt`
This file stores the sender's email and password required for sending emails.

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/mithilesh1627/Weather_Reminder_Project.git
   ```
2. Navigate to the project directory:
   ```
   cd weather-reminder
   ```
3. Install the required Python libraries:
   ```
   pip install -r requirements.txt
   ```

## Running the Scripts

### Weather Reminder on Email
To run the email reminder script:
```
python WeatherReminderEmail.py
```

### Weather Notification
To run the desktop notification script:
```
python WeatherNotification.py
```

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request with your changes.

## Contact
For any inquiries, please contact biharijarvis1627@gmail.com
