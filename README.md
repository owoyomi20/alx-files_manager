

# alx-files_manager

alx-files_manager is a simple file management API built with Express, MongoDB, Redis, Bull, and Node.js. It allows users to upload, download, delete, and list files stored on a local folder or on Google Cloud Storage. It also sends email notifications to users when their files are processed.

## Features

- Upload files to a local folder or Google Cloud Storage
- Download files from a local folder or Google Cloud Storage
- Delete files from a local folder or Google Cloud Storage
- List files from a local folder or Google Cloud Storage
- Send email notifications to users when their files are processed
- Use Redis and Bull to queue and process file operations in the background
- Use MongoDB to store file metadata and user information
- Use Express to create a RESTful API
- Use Node.js to run the server and the worker

## Installation

To install alx-files_manager, you need to have Node.js, Yarn, MongoDB, and Redis installed on your system. You also need to create a Google API with an email sending scope and a valid URL (e.g., http://localhost:5000/) as one of the redirect URIs. The credentials.json file should be stored in the root directory of this project.

Then, clone this repository and switch to the cloned repository's directory. Install the packages using `yarn install` or `npm install`.

## Usage

To use alx-files_manager, you need to set some environment variables in a file named .env. Each line should have the format Name=Value. The table below lists the environment variables that will be used by this server:

| Name | Required | Description |
| ---- | -------- | ----------- |
| GOOGLE_MAIL_SENDER | Yes | The email address of the account responsible for sending emails to users. |
| PORT | No (Default: 5000) | The port the server should listen at. |
| DB_HOST | No (Default: localhost) | The database host. |
| DB_PORT | No (Default: 27017) | The database port. |
| DB_DATABASE | No (Default: files_manager) | The database name. |
| FOLDER_PATH | No (Default: /tmp/files_manager (Linux, Mac OS X) & %TEMP%/files_manager (Windows)) | The local folder where files are saved. |
| GOOGLE_APPLICATION_CREDENTIALS | No (Default: credentials.json) | The path to the Google API credentials file. |
| BUCKET_NAME | No (Default: alx-files-manager) | The name of the Google Cloud Storage bucket where files are saved. |

After setting the environment variables, start the Redis and MongoDB services on your system and run `yarn start-server`

Source: Conversation with Bing, 6/23/2023
(1) GitHub - abybells/alx-files_manager: A simple file management API built .... https://github.com/abybells/alx-files_manager.
(2) kingsleyocran/alx-files_manager: ALX SE Project Files Manager - GitHub. https://github.com/kingsleyocran/alx-files_manager.
(3) GitHub - amanabiy/alx-files_manager. https://github.com/amanabiy/alx-files_manager.
