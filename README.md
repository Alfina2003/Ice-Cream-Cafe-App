# Ice-Cream-Cafe-App

## Description
This is a Python application designed for managing an ice cream parlor's seasonal flavor offerings, ingredient inventory, and customer suggestions regarding flavors and allergy concerns. The application utilizes SQLite for data management.

## Features
- Manage seasonal flavor offerings
- Maintain ingredient inventory
- Collect customer flavor suggestions and allergy concerns
- Maintain a cart of favorite products
- Search and filter flavor offerings
- Add allergens if they don’t already exist

## Requirements
- Python 3.x
- SQLite
- Docker (optional, for containerization)

## Description of Each File

app.py: This is the main application file where the core logic of the ice cream parlor application resides. It handles user input, displays menus, and interacts with the database.

database.py: This file contains functions for connecting to the SQLite database and creating the necessary tables for flavors, ingredients, suggestions, and the cart.

requirements.txt: This file lists all the Python packages that your application depends on. You can create this file by running pip freeze > requirements.txt after installing your dependencies.

README.md: This file provides documentation for your project, including installation instructions, usage, and any other relevant information.

Dockerfile: This file contains the instructions for building a Docker image of your application. It allows you to run your application in a containerized environment.

.gitignore: This file specifies files and directories that should be ignored by Git. Common entries include __pycache__/, .env, and any other files that should not be tracked.

## Installation

### Clone the Repository
```bash
git clone https://github.com/yourusername/ice_cream_parlor.git
cd ice_cream_parlor

### Install Dependencies

You can install the required Python packages using pip. If you have a requirements.txt file, run:
      pip install -r requirements.txt

Running the Application
Without Docker
      Ensure you are in the project directory.
      Run the application:
                 python app.py

With Docker
    1.Build the Docker image:
               docker build -t ice_cream_parlor .
    2.Run the Docker container:
               docker run -it ice_cream_parlor

Usage

Once the application is running, you will see a menu with the following options:

      Add Seasonal Flavor
      View Seasonal Flavors
      Add Ingredient
      View Ingredients
      Submit Flavor Suggestion
      Add to Cart
      View Cart
      Exit
Follow the prompts to interact with the application.
