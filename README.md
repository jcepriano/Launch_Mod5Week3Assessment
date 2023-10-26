# JeffersonCountyLibrary

## Setup
* Fork and Clone this repository
* Run `update-database`

## Exercise (12 points)

Check out a new branch and complete the following tasks **in order**:
* 2 points - There is a bug in our authentication!  Identity looks like it is set up, but we can't register users.  Find and fix this bug! (Hint: this should only take one line of code)
* 2 points - Right now, anyone can 'check out' a book.  Update the application so that only a logged in user can check out a book.
* 4 points - In this application, we have the ability to create new books.  Improve this functionality by:
  * Add a link from the nav-bar to add a book
  * Make sure only Librarians can add a book
* 2 points - Create a descriptive pull request and merge this branch into main
* 2 points - Take a screenshot of a database query result from pgAdmin that clearly shows which users in your database are librarians.  Update this README to include your screenshot below:

  ![image](https://github.com/turingschool-examples/Launch_Mod5Week3Assessment/assets/130601095/ce0d59c2-bd60-4ada-a144-42b3393c15b7)

  

## Questions (6 points)

Answer the questions below in this README.  Answer these questions as if you are in an interview!

1. What are roles and claims as they relate to Authentication and Authorization? \
   Roles are a form of authorization used to create a sort of hierarchy between different accounts in an application. Roles make it so you can authorize only certain accounts to do specific things in an application.
   For example, I could create an "Admin" role. With that, in an MVC application, I could make it so only accounts with an "Admin" role could access a specific action. Claims are pretty similar
   in this aspect. Claims are another form of authorization. Stored as key/value pairs, they use authorization based on specific attributes that can be different between accounts. A common claim is an age authenticator.
   Some websites first ask for a user's age before allowing the user to proceed to the main page, this is known as a claim. Some users may or may not be old enough to enter and interact with the website, but other users
   are. Making it so only certain users can do certain things in the app based on attributes that can change.

3. How do cookies play a role in authentication and authorization? \
   Cookies allow for information about an account to be stored and checked. They are used to determine if an account has access to specific actions based on the account's role and/or claims.
   For example, if a user logs into an application, a cookie is set containing some sort of authentication. The application can use the information stored in the cookie to authorize what the user
   can and can't access in the app. 

5. If asked to implement Auth in a new .NET application, would you use the Identity framework? \
   Yes, I would prefer to use Identity Framework instead of doing it manually. Identity Framework has a lot of code being made in the background. It also creates a user object automatically. The Identity Framework
   also generates forms for an application. There are certain aspects of it that can be tricky to work with sometimes, but the benefits of it very much outweigh the more difficult parts of using Identity Framework.

## Rubric

This assessment has a total of 18 points.  Earning 12 or higher is a pass!
