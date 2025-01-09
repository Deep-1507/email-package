
```markdown
# Email Sending Service

A lightweight package to send emails using company-specific credentials retrieved from an external API.

## Features

- Fetch email credentials dynamically using the company name.
- Send plain text or HTML emails using `nodemailer`.
- Built-in error handling for invalid or missing inputs.

---

## Installation

### Prerequisites
- Node.js and npm installed.
- External API running at:  
  `http://localhost:3000/api/email-credentials/:companyName`.

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/repository-name.git
   cd repository-name
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

---

## Usage

### 1. Import `sendMail`:
```typescript
import { sendMail } from 'your-package-path';
```

### 2. Send an email:
```typescript
sendMail({
  to: 'recipient@example.com',
  subject: 'Hello!',
  text: 'This is a test email.',
  companyName: 'YourCompanyName',
  template: '<p><b>Welcome!</b></p>', // Optional: use HTML
}).then(() => {
  console.log('Email sent successfully!');
}).catch((error) => {
  console.error('Failed to send email:', error.message);
});
```

---

## Error Handling

- **Missing credentials**: No email/password found for the company.
- **Invalid recipient**: No `to` address specified.
- **Email not sent**: Issues with the email service.

---

## License

This project is licensed under the MIT License.

---

### Author
Deependra Kumar  
[GitHub](https://github.com/Deep-1507) | [LinkedIn](https://www.linkedin.com/in/deep-fl1507/)
```

You can save this as a `README.md` file in your project repository, and it's good to go! 😊
