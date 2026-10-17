# IP Information Finder

A beginner-level networking project in Python that I built to learn how IP addresses, DNS and basic network tools work. It is written as a Jupyter Notebook with small, separate programs for each feature.

## About the Project
I started this project to understand the basics of networking by writing the tools myself instead of only reading about them. Each part of the notebook solves one small networking task, from finding my public IP to checking whether a port is open.

## Features
- IP information lookup: enter any IP address and get its country, city and ISP
- Public IP detection: finds my own public IP and shows my country, city and ISP
- Location check: checks whether I am in a specific country or city (for example Iran or Tehran)
- Website ping: sends 4 ping requests to a website and shows packet loss and response times
- Local IP detection: shows my computer's hostname and local IP address
- DNS lookup: converts a domain name (for example google.com) to its IP address
- Port checker: checks if a port (for example 80) on a domain or IP is open or closed
- Menu: a simple text menu with 7 options to choose from

## How It Works
- I used the requests library to call the free ipwho.is API, which returns IP data as JSON
- I used the socket library for the local IP, DNS lookup and port checking
- I used subprocess to run the system ping command from Python
- I added error handling with try/except and a timeout, so the program shows a clear message if there is a network problem instead of crashing

## Tech Stack
Python, requests, socket, subprocess, Jupyter Notebook

## How to Run
1. Clone the repository
2. Install the requirements: pip install requests jupyter
3. Open the notebook: jupyter notebook
4. Run the cells one by one

## What I Learned
- How IP addresses, local IPs and DNS work
- How to call a web API and read JSON data in Python
- How to use socket and subprocess for networking tasks
- How to handle network errors safely

## What I Want to Improve
- Connect all features to the menu so the program loops until I choose Exit
- Move the code from the notebook into a normal .py file
- Add input validation for IP addresses and port numbers
- Make the ping command work on Linux and macOS too (it currently uses the Windows -n option)
