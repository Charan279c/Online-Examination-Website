# Online Examination Website

## 1. Project Overview

The Online Examination Website is a web-based application developed to conduct online examinations. It allows students to log in, attend multiple-choice questions (MCQs), complete the examination within a given time limit, and view their results automatically.

The project is developed using HTML, CSS, JavaScript, and Java Servlets.

## 2. Technologies Used

- **HTML5** – Structure of the website.
- **CSS3** – Styling and responsive design.
- **JavaScript** – Client-side functionality and countdown timer.
- **Java Servlets** – Backend processing and result calculation.
- **Apache Maven** – Project build and dependency management.
- **Apache Tomcat 10.1+** – Web application server.
- **JDK 17** – Java development environment.

## 3. Features

- Student login using name and roll number.
- Multiple-choice questions with four options.
- Previous and Next question navigation.
- Countdown timer for the examination.
- Automatic submission when the timer reaches zero.
- Automatic calculation of examination results.
- Display of total marks, correct answers, wrong answers, and percentage.
- Pass/Fail result display.

## 4. Project Structure

```text
Online-Examination-Website/
│
├── pom.xml
│
└── src/
    └── main/
        ├── java/
        │   └── ExamServlet.java
        │
        └── webapp/
            ├── index.html
            ├── login.html
            ├── exam.html
            ├── result.html
            │
            ├── css/
            │   └── style.css
            │
            └── js/
                └── script.js
```

## 5. Software Requirements

Install the following software before running the project:

1. JDK 17 or later.
2. Apache Maven 3.9 or later.
3. Apache Tomcat 10.1 or later.
4. Visual Studio Code or any Java-supported IDE.
5. Web browser (Google Chrome, Microsoft Edge, etc.).

## 6. How to Run the Project

### Step 1: Verify Java Installation

Open PowerShell and execute:

```powershell
java -version
javac -version
```

Ensure that JDK 17 or later is installed.

### Step 2: Verify Maven Installation

```powershell
mvn -version
```

### Step 3: Open the Project Folder

Navigate to the project directory:

```powershell
cd "C:\Users\CHARAN\OneDrive\Desktop\Online-Examination-Website"
```

### Step 4: Build the Project

Execute the following command:

```powershell
mvn clean package
```

After successful compilation, Maven generates the WAR file inside the `target` folder.

```text
target/Online-Examination-Website.war
```

### Step 5: Deploy on Apache Tomcat

1. Locate the generated WAR file.
2. Copy `Online-Examination-Website.war`.
3. Paste it into the Tomcat `webapps` folder.
4. Start the Tomcat server.
5. Open your browser.

### Step 6: Open the Website

Enter the following URL:

```text
http://localhost:8080/Online-Examination-Website/
```

The Online Examination Website home page will appear.

## 7. Application Workflow

1. Student opens the home page.
2. Student clicks the Login button.
3. Student enters their name and roll number.
4. The examination questions are displayed.
5. Student selects answers for the MCQs.
6. The countdown timer tracks the remaining examination time.
7. Student submits the examination or the system submits it automatically when time expires.
8. The system calculates the result.
9. Student views the final examination result.

## 8. Result Calculation

The system calculates the examination result based on the student's submitted answers.

- Total Questions: 10
- Correct Answers: Number of correctly answered questions.
- Wrong Answers: Number of incorrectly answered questions.
- Unanswered Questions: Questions without selected answers.
- Score: Number of correct answers.
- Percentage: (Correct Answers / Total Questions) × 100.

## 9. Testing

The application should be tested using the following test cases:

| Test Case | Expected Result |
|---|---|
| Student login | Login successful |
| Valid examination access | Questions displayed |
| Select an answer | Answer saved |
| Navigate between questions | Questions change correctly |
| Countdown timer | Remaining time displayed |
| Submit examination | Answers submitted |
| Timer reaches zero | Automatic submission |
| View result | Score and percentage displayed |

## 10. Future Enhancements

- Admin login and dashboard.
- Database integration using MySQL.
- Multiple examination categories.
- Student registration.
- Question randomization.
- Examination history.
- Downloadable result reports.

## 11. Conclusion

The Online Examination Website provides a simple and effective platform for conducting online examinations. It reduces manual evaluation work through automatic result calculation and provides students with a convenient way to attend examinations and view their results.

---

**Project Title:** Online Examination Website

**Frontend:** HTML, CSS, JavaScript

**Backend:** Java Servlets

**Build Tool:** Apache Maven

**Server:** Apache Tomcat