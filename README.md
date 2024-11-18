# 📧 Email Sender Script

This Python script allows you to send emails with an optional file attachment using Gmail's SMTP server. It prompts the user for input such as the recipient's email address, subject, body of the email, and a file to attach. The script then sends the email securely through Gmail's SMTP server.

---

## 🛠️ Requirements

- Python 3.x
- Libraries:
  - `smtplib` (comes with Python)
  - `email.mime.multipart` (comes with Python)
  - `email.mime.text` (comes with Python)
  - `email.mime.application` (comes with Python)

---

## 📥 How to Use

1. **Clone the Repository** (if applicable):
    ```bash
    git clone https://github.com/yourusername/email-sender-script.git
    cd email-sender-script
    ```

2. **Install Dependencies** (if needed):
    - This script uses built-in Python libraries, so no external installations are necessary.

3. **Setup Gmail Account**:
    - **Important**: You must use an **App Password** instead of your Gmail account password.
    - To generate an App Password:
      1. Go to your [Google Account](https://myaccount.google.com/).
      2. Under **Security**, click on **App Passwords**.
      3. Select **Mail** as the app and **Windows Computer** (or another device) as the device.
      4. Copy the 16-character generated password.

4. **Run the Script**:
    - Open the terminal or command prompt.
    - Run the script:
      ```bash
      python email_sender.py
      ```

5. **Follow the Prompts**:
    - Enter the **recipient's email**, **subject**, **body**, and **file path** for the attachment.
    - The script will send the email with the provided information, and you'll see a confirmation message:  
      `Email sent!` 📧

---

## ⚙️ Script Workflow

1. **User Inputs**: The script prompts the user to enter:
   - Recipient's email
   - Email subject
   - Email body
   - Path to file attachment (optional)

2. **File Handling**: If a file path is provided, the script will attempt to attach the file. If no file is provided or the file is not found, the email will be sent without an attachment.

3. **Email Sending**: The email is sent through Gmail's SMTP server (`smtp.gmail.com`) using SSL for secure communication.

4. **Confirmation**: Once the email is successfully sent, you'll see:
   ```bash
   Email sent! ✅
   ```

---

## 🔐 Security

- **App Passwords**: Never use your regular Gmail password. Always generate an **App Password** for the script.
- **Sensitive Data**: Avoid hardcoding your credentials in the script. Consider using environment variables or a secure configuration file.

---

## 📄 License

This script is licensed under the [MIT License](LICENSE).

---

## 🎉 Enjoy Sending Emails! ✉️

Happy emailing! 🎉 If you encounter any issues, feel free to raise an issue in the GitHub repository.

--- 

### Example:

```bash
Please enter recipient email: example@example.com
Please enter the subject of email: Test Email Subject
Please enter the message for email: This is a test email sent from a Python script.
Please enter the file path: /path/to/your/file.txt
```

