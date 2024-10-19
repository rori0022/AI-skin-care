# AI-skin-care

while True:
    print("Login or Create Account")
    user_choice = input("Enter your choice: ")

    if user_choice == "Login":
        username = input("Enter username: ")
        password = input("Enter password: ")
        # Verify credentials
        
    elif user_choice == "Create Account":
        username = input("Enter new username: ")
        password = input("Enter new password: ")
        # Create new account
        
    print("Home Page")
    print("Navigating to Beauty Section...")
    
    print("AL Icon")
    user_click = input("Click the icon (y/n): ")
    
    if user_click.lower() == "y":
        print("Choose an option:")
        print("1. Choose Image from Gallery")
        print("2. Take Photo")
        
        user_choice = input("Enter your choice: ")
        
        if user_choice == "1":
            image = load_image_from_gallery()
        elif user_choice == "2":
            image = capture_photo()
            
        print("Analyzing image...")
        recommended_products = analyze_image(image)
        
        print("Recommended products:")
        for product in recommended_products:
            print(product)
        
    else:
        print("Exiting...")
        break
