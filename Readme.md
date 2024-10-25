
# Yummo - Your DIet Buddy 🥑💪

## Overview

Yummo is a web application that leverages AI to transform recipes based on different dietary requirements. It allows users to input recipes and convert them to various diets such as vegan, keto, gluten-free. The application uses Llamma ai with Google's to perform intelligent recipe transformations while maintaining the essence and flavor profile of the original recipe.

## Table of Contents 📑

- [Features](#features)
- [Technology Stack](#technology_stack)
- [YouTube Demonstration](#youtube-demonstration)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Support](#support)

## Features 🌟

- Add new recipes to a local database
- Transform recipes to different diets:
  - Vegan
  - Keto
  - Gluten-free
- User-friendly web interface for recipe input and transformation
- Display of both original and transformed recipes
- Real-time recipe transformation using AI


## Technology Stack
- **Backend**: Python with Flask framework
- **Database**: SQLite for local storage
- **AI Integration**: Llama ai 
- **Frontend**: HTML, CSS, JavaScript (jQuery)
- **API**: RESTful API endpoints for recipe management and transformation

## YouTube Demonstration

[Watch the video](https://youtu.be/rqy8YLz9l-w)


## Requirements
- Python 3.7 or higher
- MindsDB SDK
- SQLite3
  
## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/ai-apex-dev/yummo
    ```

2. **Create virtual env & activate it & Install required packages**:
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt
    ```

3. **Set up MindsDB**:
    - Follow the [MindsDB installation guide](https://docs.mindsdb.com/install) to install and run MindsDB locally.
    - Note the server address and port (default is `http://127.0.0.1:47334`).
    - make .env file add your Google Gemini api key 
```bash
    API_KEY='YOUR_KEY'
```
docker run -p 47334:47334 mindsdb/mindsdb
mindsdb --api=http://127.0.0.1:47334

4. **Create and populate the SQLite database**:
    ```bash
    python data.py
    ```

## Usage
1. **Run the Flask server**:
    ```bash
    flask --app main run --debug
    ```

2. **Add a recipe** by providing the recipe name and recipe text in the 'add recipe' form:
    
3. **Transform a recipe** by providing the recipe name, recipe text and selecting the desired diet in the 'transform recipe' form, and visualize the transformed recipe.

4. **Visit http://localhost:5000/get_recipes** to get all the recipes in the local database.

    
## Support 💬

If you like this project, please support it starring the GitHub repository!


Thank you for your support!
