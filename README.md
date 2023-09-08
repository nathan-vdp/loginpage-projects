# Delos Login Page
This is a front-end project for a login page named "Delos" It is designed to provide a user-friendly login interface. Please note that this project is entirely front-end-based and does not include any database or back-end functionality. Here's an overview of the code:

## Table of Contents
- Project Description
- HTML Structure
- Styling
- Usage
- Project Description
- This project represents a login page for a fictional application called "DELOS" It provides users with a login form to enter their credentials (username and password) to access the application. There is also an option to remember the user and a link to reset the password. Keep in mind this is a purely front-end web app.

## HTML Structure
The HTML file (index.html) includes the following key elements:
- **!DOCTYPE html**: Specifies the document type.
- **meta tags**: Define character encoding and responsive viewport settings.
- **script tag**: Loads the Tailwind CSS framework for styling.
- **body tag**: Sets the background image to "background-login.png" and positions the "logo.png" image in the top-left corner.
- **div element with the class "flex flex-col items-center justify-center h-screen"**: Contains the login form and centers it vertically and horizontally on the page.
- **h1 element**: Displays the text "DELOS LOG IN" with custom styling.
- **form element with the ID "loginForm"**: Represents the login form.
- **input elements**: Collect user input for the username and password. They are styled using Tailwind CSS classes.
- **Remember Me checkbox and "Forgot password?" link**: Provide options for the user.
- **button element**: Represents the login button with custom styling.

````html
<!DOCTYPE html>
<html>

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
  </head>

  <body class="bg-[url('images/background-login.png')] bg-cover">
    <img src="images/logo.png" class="fixed left-0 top-0"></img>
    <div class="flex flex-col items-center justify-center h-screen">
        <h1 class="text-3xl font-bold text-white">DELOS LOG IN</h1>
        <form class="flex flex-col" id="loginForm">
            <input type="text" name="username" placeholder="username" id="username" required
                class="bg-teal-800/50 rounded-lg placeholder-white ps-4 py-2 mt-6 text-white">
            <input type="password" name="password" placeholder="Password"
                class="bg-teal-800/50 rounded-lg placeholder-white ps-4 py-2 mt-6 text-white" id="password" required>
            <div class="mt-3">
                <input type="checkbox" name="rememberMe" class="accent-pink-100">
                <label for="rememberMe" class="text-gray-100 mr-5">Remember me</label>
                <a href="url" class="text-gray-100">Forgot password?</a>
            </div>
            <button type="submit" value="login"
                class="bg-teal-500 w-full rounded-lg mt-6 py-2 text-white">Login</button>
        </form>
    </div>
</body>

</html>
````

## Styling
The page uses Tailwind CSS for styling, which is loaded from a CDN. It applies styles such as background images, text formatting, input field styling, and button styling to create an appealing and functional login interface.

## Usage
To see how this login page looks: