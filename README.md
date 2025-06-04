# Timestamp Microservice

A simple API project built as part of the [freeCodeCamp Back End Development and APIs](https://www.freecodecamp.org/learn/back-end-development-and-apis/) curriculum.

## Overview

This is a timestamp microservice that returns Unix and UTC timestamps for given date strings or Unix timestamps. If no date is provided, it returns the current time.

This project passes all required tests from freeCodeCamp.

## Usage

### API Endpoint

- `GET /api/:date?`

    - If `:date` is **not provided**. Returns the current Unix and UTC time:
    
    ```json
    {
      "unix": 1672531200000,
      "utc": "Mon, 01 Jan 2023 00:00:00 GMT"
    }
    ```

    - If `:date` is a **valid date string or Unix timestamp**. Returns the corresponding Unix and UTC time:
    
    ```json
    {
      "unix": 1450137600000,
      "utc": "Tue, 15 Dec 2015 00:00:00 GMT"
    }
    ```

    - If `:date` is **invalid**. Returns an error message:
    
    ```json
    { "error": "Invalid Date" }
    ```

### Live Demo & Examples

[View Live Demo](https://timestamp-microservice.coding.g2k.media/)

- `https://timestamp-microservice.coding.g2k.media/api/2015-12-25`
- `https://timestamp-microservice.coding.g2k.media/api/1451001600000`
- `https://timestamp-microservice.coding.g2k.media/api/`
- `https://timestamp-microservice.coding.g2k.media/api/invalid-date`

## Getting Started

1. **Clone the repository:**
```bash
git clone https://github.com/g2k19/timestamp-microservice.git
```

2. **Install dependencies:**
```bash
npm install
```

3. **Start the server:**
```bash
npm start
```

4. **Visit:**
```
http://localhost:3000/
```

## Credits

Project starter code and requirements by [freeCodeCamp](https://www.freecodecamp.org/).
