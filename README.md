# Email Sending Service

This package provides an API for sending emails using stored email credentials retrieved from a separate API. It securely handles email sending by fetching credentials for a specified company and using those credentials for authentication to send emails.

## Features

- **Get Email Credentials**: Fetches email credentials (username and password) for a specified company from an external API.
- **Send Email**: Sends an email to specified recipients using the retrieved credentials.
- **Template Support**: Optionally sends an HTML template or plain text email.
- **Error Handling**: Handles errors such as missing credentials or invalid inputs.

## Technologies Used

- **nodemailer**: Node.js module for sending emails.
- **axios**: HTTP client for making requests to external APIs to fetch email credentials.
- **TypeScript**: Language used for developing the package.

## Installation

### Prerequisites

Ensure you have the following installed:
- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### 1. Clone the repository

```bash
git clone https://github.com/Deep-1507/email-package.git
cd email-package
