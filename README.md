# hotel-booking
# Ask the user to enter their login details
username = input("Please enter your username: ")
password = input("Please enter your password: ")

# Check if the credentials are valid
if username == 'lindehof' and password == 'hotelbooking':
    # Display a message if the credentials are valid
    print("Login successful. Welcome to the Lindehof Hotel Booking System.")
    # Ask the user to enter their booking details
    num_rooms = int(input("Please enter the number of rooms you would like to book: "))
    num_nights = int(input("Please enter the number of nights you would like to stay: "))
    # Calculate the total cost of the booking
    total_cost = num_rooms * num_nights * 100
    # Display the total cost
    print("The total cost of your booking is " + str(total_cost) + " USD.")
else:
    # Display an error message if the credentials are invalid
    print("Login failed. Please enter valid credentials.")
    exit()
