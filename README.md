Activity 6 - Object Oriented Programming First Group Project

Overview
This file implements a simple command-line social media simulation in Python.
It allows users to register, log in, create posts, like posts, comment on posts, and change their passwords.
The system is structured using object-oriented programming, with a hierarchy of classes that separate concerns such
as user management, posting, liking, and commenting. The main interaction loop presents menus for user
registration, login, and post-related actions.

Key Components
User Class
Handles user registration, login, password management, and notification messages.
Maintains dictionaries for user accounts and public posts.

Poster Class (inherits from User)
Adds functionality for creating posts. Posts are stored both in the user's private account
data and in a public post dictionary for visibility.

Liker Class (inherits from User)
Provides the ability to like posts. Users can view all public posts and increment the like count on any post.

Comments Class (inherits from User)
Enables users to add comments to any public post. Comments are appended to the selected post's data.

SocialUser Class (inherits from Poster, Liker, Comments)
Combines posting, liking, and commenting capabilities. Adds a method to view all public posts, including their likes and comments.

mainFunction Class (inherits from SocialUser)
Implements the main application logic and user interface. Contains the main menu loop for registration,
login, and exit, as well as a user menu for post-related actions after login.

Program Entry Point
At the end of the file, an instance of mainFunction is created and its main() method is called, starting the interactive session.

Design Patterns and Structure:

Uses multiple inheritance to compose user capabilities (posting, liking, commenting).
Centralizes user and post data in dictionaries for easy access and modification.
Command-line interface with menu-driven navigation for user actions.
Role in Larger System:

This file serves as a standalone social media simulation, suitable for learning or prototyping. It could be extended or integrated
into a larger system with persistent storage, user authentication, or a graphical interface.

Made by:
-Daniel Vance Candole
-Joreese Clyde Manginsay
-Novem Austria

August 12, 2025
