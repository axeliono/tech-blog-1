# Tech It Out Blog

## Description
Tech It Out is a CMS-style blog site where developers can publish their blog posts and comment on other developer's posts as well. This application follows the MVC (Model-View-Controller) paradigm in its structure, built with Handlebars.js as the templating language, Sequelize as the ORM, and the express-session npm package for authentication.

The blog is deployed live on Heroku: https://powerful-wave-68478.herokuapp.com/

 The Homepage for a logged-in user:  |  The login/signup page:  
---| ---
 <img width="270" alt="Homepage-LoggedIn" src="https://user-images.githubusercontent.com/70179648/104854007-39b91100-58ca-11eb-8ded-96fb7babbce7.png">  | <img width="272" alt="LogIn Page" src="https://user-images.githubusercontent.com/70179648/104854027-4f2e3b00-58ca-11eb-8a49-693cc103de26.png">  

Single-post page view:  |  Logged-in users dashboard:  
---| ---
 <img width="271" alt="Single-Post" src="https://user-images.githubusercontent.com/70179648/104854519-b816b280-58cc-11eb-89ef-50698ea4a95f.png">  | <img width="274" alt="Dashboard" src="https://user-images.githubusercontent.com/70179648/104854531-c9f85580-58cc-11eb-8a3a-e2817b052707.png">  


## Installation
Clone this repository, then initialize the node package manager in the root of the project folder. From the command line, run
     
     npm install bcrypt connect-session-sequelize dotenv express express-handlebars express-session mysql2 sequelize
     
 To install all dependencies needed for the application. Change the applicable fields in the .env file to connect to your MySQL database. 
 
 ## Usage
 To use the application from the root of your project folder, run the MySQL shell command `mysql -u root -p` and enter your secure password. Then from the command line, run `source db/schema.sql`. To see if the database is there, run `show databases;` in the MySQL shell. From the CL at the root of your project folder, run `npm start` to connect to the server and visit `http://localhost:3001` to view the application.
 
 The application is deployed live on Heroku (here)[https://powerful-wave-68478.herokuapp.com/]. 
 
 Users can log in and be taken directly to their dashboard to view their posts and create a new post:
 ![LogIn-NewPost](https://user-images.githubusercontent.com/70179648/104854374-de881e00-58cb-11eb-9c6c-edabf9c826e9.gif)
 
 New users can enter their information in the form to sign up. Logged in users can comment on any post:
 ![Signup-comment](https://user-images.githubusercontent.com/70179648/104854432-4d657700-58cc-11eb-854c-934f8cd0cf92.gif)
 
 Logged in users can edit or delete any of their posts by navigating to their dashboard and clicking the 'Edit post' button under any post they wish to update/delete:
 
 ![Edit-DeletePost](https://user-images.githubusercontent.com/70179648/104854472-7dad1580-58cc-11eb-8499-b34beda621d5.gif)
 
 Users who are not logged in may still view all posts on the homepage, but cannot make any comments on posts:
 ![NotLoggedIn](https://user-images.githubusercontent.com/70179648/104854498-a3d2b580-58cc-11eb-8fb7-ff26f7f1d0ec.gif)
 
## Contributing
Made by Tatum Stafford
  * [GitHub Profile](https://github.com/tmstafford)
