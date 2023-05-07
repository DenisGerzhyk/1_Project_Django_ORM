# 1_Project_Django

This is a code snippet for a Django project that involves creating a Clients model, implementing views for creating and displaying Clients objects, and setting up the project's URLs.

The Clients model has five fields: name, surname, email, number, and address. The __str__ method is overridden to return the client's name and surname as a string.

In views.py, the index function handles GET and POST requests for the index page. For a POST request, it creates a ClientsForm object with the data from the request, validates it, saves the object, and redirects the user to the display view. For a GET request, it creates an empty ClientsForm object and renders the index.html template with the form as context.

The display function retrieves all Clients objects from the database and renders the display.html template with the objects as context.

In urls.py, two URLs are defined: an empty URL that maps to the index view, and a display/ URL that maps to the display view.
