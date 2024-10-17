# QuickStatements 3.0 - Home Page Features 

The QuickStatements 3.0 homepage provides an interface for users to manage and interact with Wikidata batches. The page is divided into different sections, each with specific functionalities.

## 1. Navigation Bar
The navigation bar at the top of the page contains links to different parts of the QuickStatements application:

- **QuickStatements 3.0**: This is the main title, and clicking it takes the user back to the homepage.
- **New Batch**: A link for creating a new batch of commands to be executed on Wikidata. This is the primary feature for submitting new sets of statements.
- **Last Batches**: A placeholder link for accessing the last batches that were processed. Currently, this functionality is disabled, so the link does not perform any action.
- **Git**: A link to the [QuickStatements3 GitHub repository](https://github.com/WikiMovimentoBrasil/quickstatements3). Here, users can access the source code, report issues, or contribute to the project.

## 2. User Menu
The user menu changes based on the user's authentication status:

- **Anonymous Users**:
  - **Login**: Displays a login option for users who are not authenticated. The link is present, but it does not lead to a functional login page in this setup.
  
- **Logged-in Users**:
  - **User Profile**: Displays the username of the authenticated user. It serves as an indication of the current session's user.
  - **Your Last Batches**: A placeholder link intended to show the user's recent batches, but this feature is also currently non-functional.

## 3. Content Section
The content section (`{% block content %}`) is a placeholder in the layout file. This is where dynamic content will be loaded depending on the user's actions or the active page. For instance, when a user creates a new batch, the content displayed here would change to reflect that functionality.

## 4. Styling and Structure
The application is using a combination of Pico CSS and a custom stylesheet (`home.custom.css`). The `home.custom.css` can be used to override or customize the styles further.

- **Color Scheme**: The default styling is managed by the Pico CSS framework, which provides a modern look and feel.
- **Spinner**: An image (`spinner.svg`) is used as an indicator for asynchronous operations. It appears whenever the `htmx` library triggers an action requiring user feedback.

## 5. JavaScript
The `htmx` library is included in the page for enabling HTML-based dynamic content without needing a full page reload. This makes the interface more responsive.

## 6. Notes
- Several features, such as "Last Batches" and "Login," are placeholders and may not work in the current setup.
- The layout is structured to allow easy extension by placing content within the defined `{% block content %}` for future development.

