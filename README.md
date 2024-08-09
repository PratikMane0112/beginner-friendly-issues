# Beginner Friendly Issues to Contribute to Open Source

![t](https://github.com/user-attachments/assets/2c6274cf-9c8a-4d77-87ae-e4ea72bac8e9)

Contributing to open source can be a rewarding way to learn, teach, and build experience. Here are some beginner-friendly issues you can tackle to make valuable contributions to open-source projects.

## 1. Adding the Favicon

Favicons are the small icons that appear in the browser tab. Adding a favicon is a simple but important task.

**Steps to Add a Favicon:**

1. Create or download a favicon image (16x16 or 32x32 pixels).
2. Save it as `favicon.ico` or a suitable image format like `.png`.
3. Add the following line in the `<head>` section of your HTML file:

```html
<link rel="icon" href="path/to/favicon.ico" type="image/x-icon">
```

## 2. Adding a 404 Error Page

A custom 404 error page improves user experience when they land on a broken or non-existent link.

**Steps to Add a 404 Error Page:**

1. Create a new HTML page named 404.html.
2. Design the page with a friendly message and navigation options.
3. Configure your server or hosting service to serve this page for 404 errors.

```html
<h1>Oops! Page Not Found</h1>
<p>The page you are looking for does not exist.</p>
<a href="/">Go to Home</a>
```

## 3. Making Pages Responsive

Responsive design ensures your website looks good on all devices.

**Steps to Make Pages Responsive:**

1. Use media queries in your CSS to adjust styles for different screen sizes.
2. Use relative units like percentages or em instead of fixed units like px.
3. Utilize flexible grid systems or frameworks like Bootstrap.

```
@media (max-width: 600px) {
  .container {
    width: 100%;
  }
}
```

## 4. Adding Dark & Light Mode Feature

Dark mode can enhance user experience by reducing eye strain in low-light conditions.

**Steps to Add Dark & Light Mode:**

1. Define styles for both dark and light modes in your CSS.
2. Add a toggle switch to switch between modes.
3. Use JavaScript to toggle classes based on user preference.

```
body.light-mode {
  background-color: white;
  color: black;
}
body.dark-mode {
  background-color: black;
  color: white;
}
```

## 5. Adding License & Contributing Guidelines

Clearly define how others can contribute to your project.

**Steps to Add License & Contributing Guidelines:**

1. Choose a license and add a LICENSE file to your repository.
2. Create a CONTRIBUTING.md file with guidelines on how to contribute.

```
# Contributing Guidelines
1. Fork the repository.
2. Create a new branch.
3. Make your changes and commit them.
4. Submit a pull request.
```

## 6. Adding Hover Effects

Hover effects can enhance the interactivity of your website.

**Steps to Add Hover Effects:**

1. Use CSS :hover pseudo-class to define styles for hover state.
2. Add transitions for smooth effects.

```
button:hover {
  background-color: blue;
  color: white;
  transition: 0.3s;
}
```

## 7. Adding Preloader

A preloader can improve user experience by displaying a loading animation while the page loads.

**Steps to Add a Preloader:**

1. Create a preloader element and style it.
2. Use JavaScript to hide the preloader once the page loads.

```
<div id="preloader"></div>

<script>
  window.addEventListener('load', () => {
    document.getElementById('preloader').style.display = 'none';
  });
</script>
```

## 8. Adding Spinner

A spinner indicates loading processes, providing visual feedback to users.

**Steps to Add a Spinner:**

1. Create a spinner element with CSS animations.
2. Display the spinner during loading events.

```
<div class="spinner"></div>

<style>
  .spinner {
    border: 4px solid rgba(0, 0, 0, 0.1);
    border-top: 4px solid blue;
    border-radius: 50%;
    width: 40px;
    height: 40px;
    animation: spin 1s linear infinite;
  }

  @keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
  }
</style>
```

## 9. Enhancing the Cursor

A custom cursor can make your website more engaging.

**Steps to Enhance the Cursor:**

1. Define custom cursor styles using CSS.

```
body {
  cursor: url('path/to/cursor.png'), auto;
}
```

- Also you can use my npm package ["react-jumbo-cursor"](https://www.npmjs.com/package/react-jumbo-cursor)
  

## 10. Adding Form Validations

Form validations ensure that users submit correct and complete information.

**Steps to Add Form Validations:**

1. Use HTML5 validation attributes like required, pattern, etc.
2. Add JavaScript for custom validations.

```
<form id="myForm">
  <input type="email" required>
  <input type="submit">
</form>

<script>
  document.getElementById('myForm').addEventListener('submit', (event) => {
    if (!event.target.checkValidity()) {
      event.preventDefault();
      alert('Please fill out the form correctly.');
    }
  });
</script>
```

## 11. Adding a Scroll to Top Button

A "Scroll to Top" button enhances user experience by allowing easy navigation back to the top of the page.

**Steps to Add a Scroll to Top Button:**

1. Create a button element in your HTML file.
2. Style the button with CSS to position it fixed at the bottom right corner.
3. Add JavaScript to handle the scroll functionality.

```html
<!-- Scroll to Top Button -->
<button id="scrollToTopBtn">Scroll to Top</button>
<script>
  // Get the button
  var mybutton = document.getElementById("scrollToTopBtn");

  // When the user scrolls down 20px from the top of the document, show the button
  window.onscroll = function() {
    if (document.body.scrollTop > 20 || document.documentElement.scrollTop > 20) {
      mybutton.style.display = "block";
    } else {
      mybutton.style.display = "none";
    }
  };

  // When the user clicks on the button, scroll to the top of the document
  mybutton.onclick = function() {
    document.body.scrollTop = 0;
    document.documentElement.scrollTop = 0;
  };
</script>
```
