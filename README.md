# Web-Crawler
“A Digital Watchdog” is an innovative project designed to aggregate, filter, and present news from multiple cybersecurity and technology sources. Leveraging web scraping techniques, the system fetches the latest news articles from reputable platform as Krebs on Security, The Hacker News, Ars Technica, and TechRadar. Built using Flask, BeautifulSoup, and Python, the application provides an API endpoint (/api/scrape) that serves the aggregated news data in a structured JSON format.
Key features of the project include:
•	Multi-Source Aggregation: Scrapes news from various cybersecurity and technology websites.
•	Content Filtering: Allows users to filter news based on categories like tech, malware, and ransomware.
•	Sorting Mechanism: Enables sorting of news articles in ascending or descending ordeAr based on titles.
•	CORS Enabled API: Facilitates cross-origin requests, allowing seamless integration with frontend applications.
•	Error Handling: Robust mechanisms to handle network-related errors and ensure reliable data retrieval.

# Requirements
•	Latency:
Fetching and displaying up to 20 news articles will take less than 200 milliseconds on average.Initial API calls or scraping will execute in under 2 seconds for up to 3 sources simultaneously.

•	Memory Utilization:
Backend memory usage will not exceed 30% of an 8 GB system, even under high traffic.

•	Concurrency:
Supports simultaneous requests from up to 20 users without significant performance degradation.

•	Scalability:
Performance improves linearly with additional server resources (e.g., multi-core CPUs or increased bandwidth).

# Modules
The system is divided into the following major modules:
1.	Web Scraping Module:
o	Function: Extracts news articles from predefined sources using specific CSS selectors.
o	Technologies: Python, BeautifulSoup, Requests.
2.	Data Processing Module:
o	Function: Processes and structures the scraped data, handling tasks like content filtering and sorting.    
o	Technologies: Python.
3.	API Module:
o	Function: Provides RESTful API endpoints to serve the processed news data.
o	Technologies: Flask, Flask-CORS.   
4.	Frontend Module:
o	Function: (Assumed based on index.html) Provides a user interface to interact with the API.
o	Technologies: HTML, CSS, JavaScript.    
5.	Error Handling Module:
o	Function: Manages exceptions and ensures the reliability of data retrieval.
o	Technologies: Python exception handling.

Organise the files according to Python's structure of hosting the website, into two folders of 'static' and 'templates' and finally run the 'app.py' file to host the website on localhost(127.0.0.1/port).
