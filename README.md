# Amazon-Web-Scraping
Description

This project is designed to monitor the price of a specific product on Amazon. It checks the price and sends an email notification if the price drops below a specified threshold.
Features

    Extract product information (title and price) from an Amazon webpage.
    Record product data into a CSV file.
    Send an email notification if the price falls below the set threshold.

Installation

To work with this project, you will need the following Python libraries:

    beautifulsoup4
    requests
    pandas
    smtplib

Install them using pip:

    pip install beautifulsoup4 requests pandas

Setup

    Update Variables:
        Replace 'yourmail@gmail.com' and 'yourpassword' in the send_mail() function with your actual email address and password.
        Make sure you have enabled access for less secure apps for your Gmail account or use an app-specific password.

    Update URL:
        Replace the URL in the check_price() and get_price() functions with the URL of the product you want to monitor on Amazon.

    Configure Recipient:
        In the send_mail() function, replace 'recipient@example.com' with the email address where you want to send notifications.

Usage

    Run the Script:

    Start the script to begin monitoring the price:

    bash

    python your_script_name.py

    The script will periodically check the price of the product and send an email notification if the price drops below $15.

Notes

    Price Checking: Prices can fluctuate, so ensure the product URL and threshold price are set correctly.
    Gmail Usage: To send emails through Gmail, you may need to adjust your account security settings.

Examples

After running the script, if the product price drops below $15, you will receive an email notification.
