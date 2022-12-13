# Book-Search-Engine-with-Graghql-API

In this challenge we were to take a fully functioning Google Books API search engine built with a RESTful API, and refactor it to be a GraphQL API built with Apollo Server. The app was built using the MERN stack, with a React front end, MongoDB database, and Node.js/Express.js server and API. It's already set up to allow users to save book searches to the back end.

To fulfill the Challenge, it was required that we do the following:

1. Set up an Apollo Server to use GraphQL queries and mutations to fetch and modify data, replacing the existing RESTful API.

2. Modify the existing authentication middleware so that it works in the context of a GraphQL API.

3. Create an Apollo Provider so that requests can communicate with an Apollo Server.

4. Deploy the application to Heroku.

# A) The user story for the project was as follows:

AS AN avid reader

I WANT to search for new books to read

SO THAT I can keep a list of books to purchase

# B) The acceptance criteria for the project was as follows:

GIVEN a book search engine

WHEN I load the search engine

THEN I am presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button

WHEN I click on the Search for Books menu option

THEN I am presented with an input field to search for books and a submit button

WHEN I am not logged in and enter a search term in the input field and click the submit button

THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site

WHEN I click on the Login/Signup menu option

THEN a modal appears on the screen with a toggle between the option to log in or sign up

WHEN the toggle is set to Signup

THEN I am presented with three inputs for a username, an email address, and a password, and a signup button

WHEN the toggle is set to Login

THEN I am presented with two inputs for an email address and a password and login button

WHEN I enter a valid email address and create a password and click on the signup button

THEN my user account is created and I am logged in to the site

WHEN I enter my account’s email address and password and click on the login button

THEN I the modal closes and I am logged in to the site

WHEN I am logged in to the site

THEN the menu options change to Search for Books, an option to see my saved books, and Logout

WHEN I am logged in and enter a search term in the input field and click the submit button

THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site and a button to save a book to my account

WHEN I click on the Save button on a book

THEN that book’s information is saved to my account



WHEN I click on the option to see my saved books

THEN I am presented with all of the books I have saved to my account, each featuring the book’s title, author, description, image, and a link to that book on the Google Books site and a button to remove a book from my account

WHEN I click on the Remove button on a book

THEN that book is deleted from my saved books list

WHEN I click on the Logout button

THEN I am logged out of the site and presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button  

# C) Below is a mock-up displaying the expected functionality of the project

![21-mern-homework-demo-01](https://user-images.githubusercontent.com/108309963/207435926-845da3be-af88-4f40-852e-48ba22d3557c.gif)

 1. In the animation above, a user can type a search term (in this case, "star wars") in a search box and the results appear
 
 ![21-mern-homework-demo-02](https://user-images.githubusercontent.com/108309963/207436216-18c1d053-2f27-41c0-984d-405aa19bb784.gif)
 
 2. In the animation above, the user can save books by clicking "Save This Book!" under each search result, as shown in the following animation
 
 ![21-mern-homework-demo-03](https://user-images.githubusercontent.com/108309963/207436429-98e0f2c4-05a5-4371-aed5-3702a6b1e091.gif)
 
 3. A user can view their saved books on a separate page, as shown in the animation above
 
 # D) The link below shows the deployed app on heroku and the app's actual functionality:
 

