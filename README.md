# RedisLoginPost

Web Application that allows users to register, login and post data. 

## How it works

Users register using a script formatted using HTML and CSS. The logic behind this script is jQuery. Depending on whether the user
is logging in or registering the script will show different information. If the user is registering a name field will be shown
to allow the user to input their name. Users input information into input fields. The JSON data is then routed over to the Node.js script. This data is then checked against the MySQL Database
to see if the user already exists or is a new user. If it's a new user the user can't log on. Once the user has registered they 
will be able to log on. This log on data is saved in a Redis Database. This allows the user's information to persist even
when routed to different webpages. Once the user logs on the user will be routed to a new page where they can post data. The 
user inputs data and this data will be saved in a separate table in the MySQL database. Users are notified using an alert message
depending on their actions.
