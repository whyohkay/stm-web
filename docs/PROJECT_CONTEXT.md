# Smart Task Manager project details

Smart Task Manager uses Flutter/Dart for the interface, FastAPI for the backend and PostgreSQL for storage. The project also used Docker. This repository contains the compiled Flutter web build deployed to GitHub Pages.

## My contribution

I used AI assistance to build the application. The project helped me understand how the Flutter interface connects to the API and how the backend uses the database.

## Web deployment

`index.html` loads the application under `/stm-web/`. Flutter startup files load the compiled Dart bundle and rendering assets. The editable Dart application, API source and database configuration are not included here.

## Push notifications

`serviceworker.js` displays incoming push notifications and opens or focuses the application when a notification is clicked. Notifications require backend delivery and a configured browser subscription.
