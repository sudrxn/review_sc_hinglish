# Flask Review Scraping Application

This Flask application scrapes product reviews from Flipkart using BeautifulSoup and stores them in a MongoDB database.

## Prerequisites

Before running the application, ensure you have the following installed:

- Python 3.x
- Flask
- Flask-Cors
- requests
- BeautifulSoup (bs4)
- pymongo
- MongoDB

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your/repository.git
   cd repository
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up MongoDB:
   - Create a MongoDB database and collection.
   - Update the MongoDB connection string (`client = pymongo.MongoClient(...)`) with your credentials.

## Usage

1. Run the Flask application:
   ```bash
   python app.py
   ```
   The application will start on `http://127.0.0.1:8000/`.

2. Navigate to `http://127.0.0.1:8000/` in your web browser to access the home page.
   
3. Enter a product name in the search box and submit the form to fetch and store reviews from Flipkart.

## Features

- **Home Page**: Displays a simple UI to enter a product name for review scraping.
- **Review Scraping**: Scrapes reviews for the specified product from Flipkart.
- **Data Storage**: Stores scraped reviews in a MongoDB database.
- **Error Handling**: Catches exceptions during scraping and displays an error message.

## File Structure

```
├── app.py                    # Main Flask application file
├── templates/                # HTML templates
│   ├── index.html            # Home page template
│   └── results.html          # Results page template
└── README.md                 # Documentation file (you are here)
```

## Contributing

Contributions are welcome! If you have any suggestions or improvements, please create a pull request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
