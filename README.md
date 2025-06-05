# 📧 Spring Boot Email Sender

This project demonstrates how to send emails using **Spring Boot** and **Gmail SMTP** with the `JavaMailSender`.

---

## 🚀 Features

- ✅ Send simple plain-text emails
- ✅ REST API endpoint to send emails
- ✅ Gmail SMTP integration
- ✅ Easy to use and lightweight

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot 3.x
- Maven
- Gmail SMTP

---

## 📁 Project Structure

```
spring-boot-email/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/example/email/
│       │       ├── controller/
│       │       │   └── EmailController.java
│       │       ├── service/
│       │       │   └── EmailService.java
│       │       └── SpringBootEmailApplication.java
│       └── resources/
│           └── application.properties
├── pom.xml
└── README.md
```

---

## ⚙️ Setup Instructions

### 🔹 Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/spring-boot-email-sender.git
cd spring-boot-email-sender
```

---

### 🔹 Step 2: Add Email Configuration

Update your `src/main/resources/application.properties`:

```properties
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=your_email@gmail.com
spring.mail.password=your_app_password
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true
```

> 💡 **Note:** Use [App Passwords](https://support.google.com/accounts/answer/185833) for Gmail if 2-step verification is enabled.

---

### 🔹 Step 3: Run the Application

```bash
./mvnw spring-boot:run
```

---

## 📬 API Usage - Send Email

### 🔸 API Endpoint

```
POST http://localhost:8080/api/email/send
```

### 🔸 Parameters

| Parameter | Type   | Description             |
|-----------|--------|-------------------------|
| toEmail   | String | Recipient email address |
| subject   | String | Subject of the email    |
| body      | String | Content of the email    |

---

## 📮 Postman Example

You can test the API using Postman or any browser by sending a GET request like this:

```
http://localhost:8080/email/send?to=sendersmail@gmail.com&subject=Hello Hr&body=Hi this is a test
```

> 📨 Replace `sendersmail@gmail.com` with the actual recipient email address.

---

## 📹 YouTube Tutorial

📺 [Send Email using Spring Boot | Gmail SMTP | Java Mail Sender](https://youtu.be/42rA_GOlLHA?si=lZEl6GzSXlLwvZsv)

---

## 👨‍💻 Author

**Sharad Kamble**  
GitHub: [@sharad-kamble](https://github.com/sharad-kamble)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---