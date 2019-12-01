# RESTful Client
Project to learn on Restful client requests. You need to run Flask_service.py before running the following activites as Flask_service.py are the flask services we created before.

## Project 1:
Project to learn on Get request
Steps:
* Send a GET request (URL: " http://127.0.0.1:5000/books ") and get the books ordered by 'Date_of_Publication' in an ascending order
* Print the status code (HTTP response code) of response object
* Convert the content of the response object to a python dictionary
* Print top 5 books

## Project 2:
Project to add new book
Steps:
* Create a python dictionary with the expected keys and custom values.

{
  "Date_of_Publication": 0,
  "Publisher": "string",
  "Author": "string",
  "Title": "string",
  "Flickr_URL": "string",
  "Identifier": 0,
  "Place_of_Publication": "string"
}
    
* Send a POST request (URL: " http://127.0.0.1:5000/books ") and use send the book as the request payload
* Print the status code and the message returned by the service

## Project 3:
Project to update the book with its ID
Steps:
* Send a get request to get the book with id=206 (URL: " http://127.0.0.1:5000/books/206 "), and print the book
* Update the author to 'Nobody'
* Send a PUT request to update the book
* Print the status code and the message returned by the service
* Once again, send a get request to get the book with id=206 (URL: " http://127.0.0.1:5000/books/206 ") and print the returned book to see if the book has been successfully updated

## Project 4:
Project to delete the book with its ID
Steps:
* Send a get request to get the book with id=206, and print the book
* Send a delete request (URL: " http://127.0.0.1:5000/books/206 ") to remove the book with id=206
* Print the status code and the message returned by the service
* Once again, send a get request to get the book with id=206 to see if the book doesn't exist
