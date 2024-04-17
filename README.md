# OTP Verification System

This OTP Verification System is a simple simulation of a server that generates and verifies Time-based One-Time Passwords (TOTPs). The system comprises three main components:

- Server (server.py): Generates OTPs and verifies them upon client requests.
- Client (client.py): Periodically requests new OTPs from the server every 30 seconds.
- End-User (user_input.py): Allows a user to manually input an OTP to be verified by the server.
		
# Features
- OTP Generation: Dynamically generate a TOTP using a fixed secret key.
- OTP Verification: Validate the OTP entered by the end-user against the server.
- Periodic OTP Request: Simulate an application requesting OTPs in regular intervals.

# Requirements
Python 3.6 or higher
pyotp library

# How It Works
- The server generates an OTP upon a client's request and sends it to the client. It also listens for OTPs sent for verification and responds whether they are valid or not.
- The client periodically requests OTPs from the server and prints them out. This simulates an external system like an app receiving OTPs.
- The end-user script allows users to enter an OTP, which is then sent to the server for verification. The server's response (valid or invalid) is displayed to the user.
