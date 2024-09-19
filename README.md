# URL Shortener

## Overview
This is a simple URL Shortening Service developed in Java that allows users to shorten long URLs into compact, shareable links. The service also tracks how many times each shortened URL has been accessed. It features:
- URL validation (ensures that URLs start with "http" or "https")
- Generation of a random 6-character short URL key
- URL history display (shows shortened URLs and their access counts)

## Features
- **URL Shortening**: Shorten a valid long URL into a short, unique URL.
- **Original URL Retrieval**: Retrieve the original long URL using the short URL.
- **URL Access Tracking**: Track how many times each short URL has been accessed.
- **History Display**: View all shortened URLs and their respective access counts.

## Technologies Used
- **Java**: The application is written in Java using basic Java utilities such as `HashMap`, `Scanner`, `Random`, and `Pattern`.
- **Data Structures**: `HashMap` is used to store mappings between long URLs and short URLs, as well as to track access counts.
- **Regular Expressions**: The `Pattern` class is used for URL validation.
  
## How It Works
1. **URL Shortening**:
   - User provides a long URL (e.g., `http://example.com`).
   - The application checks if the URL is valid (it must start with `http://` or `https://`).
   - If the URL is valid, a 6-character short URL is generated using a combination of uppercase, lowercase letters, and numbers.
   - The short URL is stored along with the long URL, and the system initializes the access count to 0.

2. **URL Retrieval**:
   - The user provides the short URL (e.g., `http://short.ly/abc123`).
   - The application looks up the long URL associated with the short URL.
   - Each time a short URL is accessed, the access count is updated.

3. **History Display**:
   - The application lists all shortened URLs along with their original URLs and the number of times they have been accessed.


