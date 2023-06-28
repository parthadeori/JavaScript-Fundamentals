# **Linking a JavaScript File**

To link a JavaScript file to an HTML document and view it in a web browser, follow the steps below.

## **Prerequisites**

Ensure that you have the following software installed on your computer:

* **A text editor** (e.g., Visual Studio Code, Sublime Text)
* **A web browser** (e.g., Google Chrome, Mozilla Firefox)

## **Steps**

* Open your text editor.
* Create a new HTML file and save it with a .html extension (e.g., index.html).
* Create a new JavaScript file and save it with a .js extension (e.g., script.js).
* Open the HTML file in your text editor.
* Add the following code within the <head> section of your HTML file to link the JavaScript file:

**HTML File**
```
<!DOCTYPE html>
<html>
<head>
  <title>My Web Page</title>
  <script src="script.js"></script>
</head>
<body>
  <!-- The rest of your HTML content goes here -->
</body>
</html>
```

* Save the changes to your HTML file.
* Open the JavaScript file (`script.js`) in your text editor and add your JavaScript code:

**JavaScript File**
```
console.log("Hello, World!");
```

* Save the changes to your JavaScript file.
* Open the HTML file in your preferred web browser.
* Open the browser's developer console by right-clicking anywhere on the page and selecting Inspect or using the shortcut Ctrl + Shift + I (Windows/Linux) or Cmd + Option + I (macOS).
* In the console, you should see the output from your JavaScript code.

Congratulations! You have successfully linked a JavaScript file to an HTML document and viewed it in a web browser.

You can now write and execute more JavaScript code within the linked JavaScript file to enhance your web page's functionality. Happy coding! 🎉💻
