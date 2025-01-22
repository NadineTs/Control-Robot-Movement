# Control-Robot-Movement

## overview 
This project enables users to control a robot's movement through a web interface. It features an HTML front-end and a PHP back-end that interacts with a MySQL database to log movement commands.


## Setup Instructions

1. **Install XAMPP**:
   - Download and install XAMPP from the official website.
   - Start the Apache and MySQL modules from the XAMPP Control Panel.

2. **Create the Database**:
   - Open phpMyAdmin by navigating to `http://localhost/phpmyadmin` in your web browser.
   - Create a new database named `robot_control`.
   - Execute the following SQL command to create a `movements` table:
     ```sql
     CREATE TABLE movements (
         id INT(11) AUTO_INCREMENT PRIMARY KEY,
         direction VARCHAR(255) NOT NULL,
         timestamp TIMESTAMP DEFAULT CURRENT_TIMESTAMP
     );
     ```

3. **Set Up the Project Files**:
   - Create a new folder in the `htdocs` directory of your XAMPP installation (e.g., `C:\xampp\htdocs\robot_control`).
   - Save the provided HTML and PHP code in this folder:
     - Name the HTML file `index.html`.
     - Name the PHP file `update.php`.
     - Name the PHP file `get_last_direction.php`.

4. **Access the Application**:
   - Open your web browser and navigate to `http://localhost/robot_control/index.html`.
   - You should see the robot control interface.
  


  ## Usage
- Click the directional buttons to send movement commands to the robot.
- The application logs the last direction sent to the database, which can be retrieved for reference.



![Image](https://github.com/user-attachments/assets/c67c6e63-cf61-491d-a594-36c22d450aed)

![Image](https://github.com/user-attachments/assets/dbf72baa-5c34-49c4-81bd-e8c1c4df816c)
