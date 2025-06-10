# food-ordering-and-delivery-management-system
food ordering delivery system
# Food-Ordering-Website
A food ordering website made using Java, JDBC, JSP and servlets.

We made this project during my 2nd semester for my OOPS Java course. We were supposed to use JSP and Servlets for the same.
The website was on local host using Tomcat server. JDBC and MYSQL were used to create a database for the application.
<br>
<br>
We will now walk you through the different webpages and features of the website.
All the images used for the project were copyright free when we used them. If they do belong to someone let me know and we will  remove them.
<br>
<br>
## 📌 Features

- User Registration & Login
- Browse and Search Food Items
- Add to Cart and Place Orders
- Track Order Status
- Admin Panel for Food and Order Management
- Real-time Data Handling with MySQL
  
## 🛠️ Technologies Used

| Technology       | Description                              |
|------------------|------------------------------------------|
| **Java (JDK 8+)**| Core programming language for logic       |
| **Swing**        | Java GUI framework for building UI       |
| **MySQL**        | Relational database for storing records  |
| **JDBC**         | Java API for connecting to MySQL         |


### Login Page
This is a simple html page which has a form and uses 'post' method to pass on the form values to ***loginCheck.java*** for validating login.
One can also register a new account if they don't have an existing account.

![A screenshot of the login page](![Screenshot 2025-05-24 002421](https://github.com/user-attachments/assets/fe036122-1a16-45ae-8bf7-f6327a745b11)
)

<br>

### Register Page
This page is again using a form to get information from the user using 'post' method to pass on the form values to ***registerInput.java*** for registering the new user and making a corresponding entry in the database. Certain constraints were put on values being entered for the email and password to verify they're in the correct format and adequate length using **regex**. 

![A screenshot of the register page](![Screenshot 2025-05-24 004143564](https://github.com/user-attachments/assets/36623bde-a223-4584-b54c-47ef7dd01f04)
)

After entering the required information and clicking on the Register button the user is redirected back to the login page where they can login using their registered email id and password.

![A screenshot of the login page](![Screenshot 2025-05-24 0046519999](https://github.com/user-attachments/assets/9e165d02-12bd-45c9-b02b-180ca6ea974a)
)

### Welcome Page
Once the user has successfully logged in they will be taken to the menu page i.e. ***Welcome.jsp*** and the users session will start. This page has a navigation bar with a logout button and a button to go to the cart.
Further it has multiple containers with the images of various food items with buttons to add them to cart. If a user clicks on logout their session ends and they're redirected to the login page.
If a user clicks on the **Add to Cart** button a value is passed to ***addToCart.jsp*** this program adds the item to cart while the user is still on the menu page. A user can add multiple items to their cart.

![A screenshot of the Welcome page](![Screenshot 2025-05-24 00494677777](https://github.com/user-attachments/assets/aff03995-f623-4e2f-b5a8-a00dd6cc34bb)
)

### Cart Page
When the user clicks on **Cart** button on the navigation bar they're taken to ***cart.jsp*** where the added items are shown to the user.
![A screenshot of the Cart page](![Screenshot 2025-05-24 0052056666](https://github.com/user-attachments/assets/312f176b-49da-48f6-a723-6027368d5802)
)

From this page the user can either go back to the menu page to add more items by clicking on **Continue Shopping** button or click on **Checkout** Button. 
### Checkout Page
On clicking the checkout button the user is taken to ***Checkout.jsp*** page. On This page the user has only one option that is to logout.
![A screenshot of the Checkout page](![Screenshot 2025-05-24 005400](https://github.com/user-attachments/assets/54fc3a4e-3ba0-4902-8d07-4bf52728492b)
)

<br>
<br>
<br>
Now, coming to the database part of the application. I used MYSQL to create my database and tables. It was connected to my java code using JDBC.
The following are the tables which were created in the db.

![](![Screenshot 2025-05-24 005740](https://github.com/user-attachments/assets/a335feac-8633-424d-aa3a-b77b3c122705)
)

### customer table
Schema is as follows

(![Screenshot 2025-05-24 010003](https://github.com/user-attachments/assets/7e300cd2-34fd-4a28-b020-4e9a564c68b1)
)

### drinks table
Schema is as follows

(![Screenshot 2025-05-24 005951](https://github.com/user-attachments/assets/77c6e1a8-d147-4001-a47e-2e8aec1fe984)
)

### food table
Schema is as follows

(![Screenshot 2025-05-24 005939](https://github.com/user-attachments/assets/47e753b0-ff93-4bbf-bc31-6cf5d3889596)
)

### drinkOrder table
Schema is as follows

(![Screenshot 2025-05-24 005931](https://github.com/user-attachments/assets/30ed3009-3853-44d9-b53b-e313785b3a31)
)

### foodOrder table
Schema is as follows

(![Screenshot 2025-05-24 005920](https://github.com/user-attachments/assets/1e144e4c-35bd-4675-843d-364f5065faf1)
)

### totalOrder table
Schema is as follows

(![Screenshot 2025-05-24 005910](https://github.com/user-attachments/assets/cbf161af-44d3-440d-84dc-0472a481f748)
)
