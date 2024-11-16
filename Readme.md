# Citizens Bank Website - Local Setup Guide

This is a simple static website for **Citizens Bank** that you can run locally on your computer. Follow these steps to get it up and running, including how to set up Sass for styling.

## Prerequisites

- You don’t need any special software to run this project — just a browser and a text editor (if you want to modify the files).
- **For Sass**: If you plan to work with Sass (to modify styles), you’ll need to install Node.js and Sass.

## Steps to Run Locally

### 1. **Download the Code:**
   - First, download the entire project folder (including HTML, images, and CSS files). You can do this by either cloning the repository or manually downloading it.

### 2. **Open the Project Folder:**
   - Navigate to the folder where you downloaded the project. Inside, you should see the following structure:
     ```
     citizens-bank-website/
     ├── images/            # Folder containing images
     ├── css/               # Folder containing the styles.css file
     ├── index.html         # Main HTML file
     ├── README.md          # This file you're reading
     └── sass/               # Folder containing Sass (.scss) files
     ```

### 3. **Open the HTML File in Your Browser:**
   - Open the `index.html` file in any modern web browser (Google Chrome, Firefox, Safari, Edge, etc.). You can do this by:
     - Right-clicking on the file and selecting **Open With** → **[Your Browser]**, or
     - Dragging and dropping the file directly into your browser window.

### 4. **Sass Installation (Optional for Customization):**
   If you plan to **modify the styles** and use Sass, follow these steps to install and compile Sass.

#### a. **Install Node.js:**
   - If you don’t already have **Node.js** installed, download and install it from the official website:  
     [https://nodejs.org/](https://nodejs.org/)
   - Node.js includes **npm (Node Package Manager)**, which will allow you to install Sass and other dependencies.

#### b. **Install Sass:**
   - Once Node.js is installed, open a terminal/command prompt and run the following command to install Sass globally:
   ```bash
    npm install -g sass

#### c. **Compile Sass:**
   Once Sass is installed, you need to compile the Sass files (`.scss`) into the final CSS file. To do this:
   - Open a terminal or command prompt in the project folder.
   - Run the following command to compile Sass into CSS:
     ```bash
     sass sass/styles.scss css/styless.css
     ```
     - This command will compile the `styles.scss` file from the `sass/` folder into the `styless.css` file in the `css/` folder.
     - **Note**: If you want Sass to automatically watch for changes and update the CSS file as you modify the `.scss` files, use this command:
     ```bash
     sass --watch sass/styles.scss:css/styless.css
     ```
     This will keep the `styless.css` file updated every time you save a change in `styles.scss`.

### 5. **View the Website:**
   - Once the HTML file is open in your browser, you should see the Citizens Bank website in action. The layout includes the hero section, articles, officers' testimonials, and footer.
   - **Important Note**: If you are using Sass, the styles from the `styless.css` file (compiled from Sass) will be applied, so make sure that the file is correctly compiled and up-to-date.

### 6. **Optional - Customize and Modify:**
   - **HTML**: Open the `index.html` file in a text editor (like Notepad, Visual Studio Code, or Sublime Text).
     - Modify the content, update images, or add new sections as needed.
   - **CSS/Sass**:
     - If you're working with Sass:
       - Open the `sass/styles.scss` file to edit styles.
       - The Sass compiler (`sass --watch`) will automatically detect changes and update the `css/styless.css` file.
     - If you're not using Sass, you can directly modify the `css/styless.css` file for styling changes.
   - **Images**:
     - Replace or add new images to the `images/` folder.
     - Make sure the file paths inside `index.html` are correct to reflect any image changes.

### 7. **Troubleshooting:**
   - If the website isn't displaying properly or you don't see your style changes, here are some things to check:
     - **Images Not Displaying**: Ensure that the image paths in the HTML (`./images/`) point to the correct files in the `images/` folder.
     - **CSS Not Loading**: Make sure that the `styless.css` file is linked correctly in the `<head>` section of your `index.html` file:
       ```html
       <link rel="stylesheet" href="css/styless.css">
       ```
     - **Sass Not Compiling**: If your Sass changes are not reflecting, ensure you ran the `sass --watch` command correctly and that the Sass files are saved with a `.scss` extension.
     - **Sass Installation Issues**: If you encounter issues with Sass not being recognized in the terminal, you may need to install Sass globally again:
       ```bash
       npm install -g sass
       ```

### 8. **Test Responsiveness (Optional):**
   - Open the website in your browser and test how it looks on different screen sizes (resize your browser window).
   - The website includes media queries to ensure it's responsive on mobile, tablet, and desktop screens.
   - You can make adjustments to the media queries in the Sass files (`sass/styles.scss`) to change the layout for different screen sizes.

## Notes

- This is a **static website** that doesn’t require any server-side technologies.
- If you make any changes to the HTML or CSS (via Sass), just refresh the browser to see the updates.
- Ensure that any external links in the HTML  are functional by checking the `href` URLs.






