# AI-skin-care

START
OPEN application
 
DISPLAY "Login or Create Account"
 WAIT FOR user choice
 
IF user chooses to login THEN
    PROMPT user for credentials
    VERIFY credentials
ELSE  user chooses to create account THEN
    PROMPT user for account details
    CREATE new account
 
DISPLAY "Home Page"
SELECT "Beauty Section"
 
DISPLAY "AL Icon"
WAIT FOR user click
 
IF user clicks icon THEN
    DISPLAY "Choose an option:"
    DISPLAY "1. Choose Image from Gallery"
    DISPLAY "2. Take Photo"
     
 IF user choice == 1 THEN
        LOAD image from gallery
 ELSE user choice == 2 THEN
        OPEN camera
        CAPTURE photo
 
    ANALYZE image
    RECOMMEND products based on analysis
    DISPLAY recommended products
  
END
