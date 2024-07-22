# go-photo-blog
This is a simple Go web server for uploading files. Uploaded files are hashed using SHA-1, stored in the public/pics directory, and listed on the index page. The filenames are stored in a cookie to maintain state across requests.

## Features
Upload files via a web form.
Store uploaded files in a server directory.
List uploaded files on the index page.
Store filenames in cookies to maintain state.

## How It Works
main.go: The main application file containing the server logic.

init(): Parses templates from the templates directory.

main(): Sets up route handlers and starts the server.

index(): Handles file uploads, saves files, updates cookies, and renders the template.

cookie(): Manages session cookies.

saveToCookie(): Adds filenames to cookies.
