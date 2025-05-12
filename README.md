<p align="center">
  <a href="https://nikshay-setu.in/" target="blank"><img src="https://nikshay-setu.in/newLogo.b72ac552416e2a050fc6c22c0491143e.svg" width="200" alt="Ni-Kshay SETU" /></a>
</p>

<div align="center">

![Static Badge](https://img.shields.io/badge/Subscribers-44k-green)
![Static Badge](https://img.shields.io/badge/Licence-GPL%203.0-blue)

</div>

## Ni-Kshay SETU | Support to End Tuberculosis

The Ni-Kshay SETU app (https://nikshay-setu.in/), already with 44K subscribers, empowers healthcare providers to make informed decisions and contributes to India's mission to combat tuberculosis. Available on web, Android, and iOS platforms in 8 languages, it offers real-time updates, interactive modules, and personalized insights, revolutionizing TB knowledge management and accessibility across India.

## Table of Contents

1. Introduction
2. Features
3. Technologies Used
4. System Requirements
5. Installation
6. Configuration
7. Usage
8. Contribution Guidelines
9. Test
10. Swagger Docs Steps
11. File Structure
12. Third party Documentation
13. License

## 1. Introduction

Ni-Kshay SETU is a groundbreaking digital solution available as a web application, Android application, and iOS application. With a mission to support healthcare providers in decision-making and transform knowledge into empowerment, this innovative and interactive learning tool is a catalyst in India's journey towards a TB-free nation. As a comprehensive digital platform, Ni-Kshay SETU revolutionizes the way healthcare providers approach TB management. By leveraging cutting-edge technology, it empowers medical professionals with real-time support and evidence-based recommendations, ensuring they have the most up-to-date information at their fingertips. With an intuitive interface and user-friendly design, Ni-Kshay SETU offers a seamless experience across devices, making it accessible to a wide range of users. The web application allows healthcare providers to access the platform from any computer, while the Android and iOS applications provide mobility and convenience for on-the-go professionals. Through a range of interactive modules, virtual simulations, and case studies, Ni-Kshay SETU transforms learning into a dynamic and engaging experience. Healthcare providers can enhance their knowledge and skills by practicing TB case management in a risk-free environment. They can diagnose, prescribe treatment plans, and monitor patient progress, gaining invaluable experience and building their confidence in TB management.

> The Ni-Kshay SETU app is part of the 'Closing the Gaps in TB care Cascade (CGC)' project, developed by the Indian Institute of Public Health, Gandhinagar (https://iiphg.edu.in/). This project aims to strengthen health systems' ability to comprehensively monitor and respond to the TB care cascade with quality improvement (QI) interventions. This digital solution is one of the key interventions of the project with the objectives to strengthen the knowledge support system of the health staff in TB patient-centric care and program management of the National TB Elimination Program.

> IIPHG, The Union, and NTEP are proud partners in the development and implementation of Ni-Kshay SETU.

> Technological support for this project is provided by Digiflux Technologies Pvt. Ltd. (https://www.digiflux.io), contributing to the development and implementation of the digital solution.

## 2. Features

- **Subscriber Monitoring:** Keep track of Ni-Kshay SETU subscribers' progress and activities.
- **Data Visualization:** Visualize data in a user-friendly way for easy analysis, making it simpler to understand complex information.
- **Module Management:** Create and manage various modules, including Diagnosis, Treatment, and other types of content to tailor the platform to your needs.
- **Assessment Creation:** Develop and manage assessments for all subscribers or specific groups, allowing for better evaluation and customization. This can also be done at each state/district levels for their respective programs.
- **Material and Document Management:** Organize and provide access to materials and documents for subscribers, ensuring they have the necessary resources.
- **Leaderboard Progress:** Monitor subscribers' progress using leaderboard parameters, encouraging healthy competition and motivation.
- **Notification System:** Implement a notification system to alert and remind subscribers about important information and activities.
- **Roles and Permissions:** Manage roles and permissions for State and District level administrators to maintain control and security.
- **Master Data Management:** Oversee master data such as states, districts, health facilities, and cadres to ensure accuracy and consistency in the system.
- **Automatic News Feed:** Incorporate an automated news feed from various sources, keeping subscribers informed and updated on relevant news and developments.
- **Central Government Applications:** Add relevant applications related to government programs, enhancing the platform's utility and functionality.
- **Multilingual Support:** Control and manage multiple language support directly from the admin panel, making it easier to serve a diverse user base.
- **Chatbot and Machine Learning:** Manage and control the chatbot, machine learning, and data modeling features, offering users an interactive and intelligent experience within the platform.
- **Managing Health Facilities for T.B. :** Efficiently manage healthcare facilities within the platform, complete with configurable locations (State, District, Village, City including Latitude Longitude) and details about the services available at each location.
- **KBase:** Provides cadre-specific learning content.
- **Knowledge Quiz:** Offers proactive and planned assessments based on user activity.
- **Query2CoE:** Enables users to raise queries related to TB treatment protocols and ensures timely responses through a structured ticketing system.
- **Screening Tool:** Assists in early identification of potential TB cases.

## 3. Technologies Used

- Back-end: Node js
- Database: Mongo DB
- Notification: Email, SMS, Firebase Push Notification Service

## 4. System Requirements

- Operating System: Windows, Linux, macOS
- Node js 20
- Mongodb
- Internet connectivity for SMS, Email & Firebase Push notifications

## 5. Installation

### Install Node version v20

Make sure you have Node.js version 20 installed. You can verify your Node.js version by running:

```
node -v
```

### Installation

```
- git clone <repository_url>
- cd <project_directory>
- npm install
```

### Starting the Server

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

### Code Formatting and Linting

```
1. Create a .eslintignore file to specify files and folders that ESLint should ignore:1. Install Prettier:
    `npm install --save-dev prettier`

2. Create a .prettierrc file in the root of your project with the following configuration:
   {
    "semi": true,
    "trailingComma": "es5",
    "singleQuote": true,
    "printWidth": 80,
    "tabWidth": 2,
    "useTabs": false
  }

3. Create a .prettierignore file to specify files and folders that prettier should ignore:
       node_modules
       dist

4. Install ESLint:
    `npm install --save-dev eslint`

5.  Initialize ESLint:
    `npx eslint --init`

6. Create a .eslintignore file to specify files and folders that ESLint should ignore:
    node_modules
    dist

7. CSpell Configuration (`.cspell.json`)
  {
    "version": "0.2",
    "language": "en",
    "words": ["nextjs", "typescript"],
    "ignorePaths": ["node_modules", "build"]
  }
```

### VSCode Integration

For a better development experience, you can install the Prettier and ESLint extensions in Visual Studio Code:

1. Open the Extensions view by clicking the Extensions icon in the Sidebar or pressing `Ctrl+Shift+X`.
2. Search for `Prettier - Code formatter` and click `Install`.
3. Search for `ESLint` and click `Install`.

Configure VSCode to format and lint on save by adding the following settings in your `settings.json`:

```
{
  "editor.formatOnSave": true,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

### Create controller service and module with CLI

```bash
# development
$ nest generate resource resource_name

Example: nest generate resource Roles
```

## 6. Configuration

The application requires certain configuration settings to work correctly. The main configuration file is `.env`. Update the following settings based on your environment:

- `MONGO_URL`: The MongoDB connection string used to connect your application to the MongoDB database.
- `JWT_SECRET`: The secret key used to sign JWT tokens. Set a strong secret in production. The current description seems incorrect — this should be a secure string, not a boolean.
- `TOKEN_EXPIRY`: Specifies how long JWT tokens should remain valid (e.g., 3600s, 1d).
- `MAIL`: Configuration for your mailing service (e.g., SMTP settings or SendGrid credentials).
- `AWS`: Configure the AWS settings.
- `FIREBASE_CREDENTIALS`: Firebase service account credentials, typically a JSON string, used to initialize Firebase SDK for push notifications or Firebase auth. (This is duplicated; see below.)
- `TEXTLOCAL_API_KEY`: API key for the TextLocal SMS provider. Used to send SMS notifications.
- `TEXTLOCAL_API_ENDPOINT`: API endpoint URL for sending SMS via TextLocal.
- `SMS_API_KEY_PROMOTION`: Possibly a separate API key or header used for promotional or OTP SMS.
- `SLACK_WEBHOOK_URL`: Slack webhook URL for sending general application notifications to a Slack channel.
- `SLACK_WEBHOOK_ALERTS_URL`: A special Slack webhook URL for sending alert notifications (e.g., system errors or ML model results).
- `SYSTEM_QA_URL`: Likely a QA (quality assurance) environment URL for the system. 4 seems incorrect — probably should be a URL.
- `CHATBOT_URL`: Endpoint for chatbot services. Current description refers to reCAPTCHA, but this seems off. Should be the chatbot’s backend URL.
- `ASSESSMENT_URL`: Frontend URL used for sending automatic assessment-related notifications.
- `NTEP_URL`: S Backend URL related to NTEP (possibly a health program or system).
- `MANAGE_TB_URL`: Backend URL for managing TB (tuberculosis) cases.
- `QUESTION_URL`: Backend URL for question management service.
- `NTEP_CRED`: Credentials for accessing NTEP services/APIs.
- `QUESTION_AUTH`: Authentication details for accessing question services. Likely a token or credential.
- `COURSE_NTEP_API`: API URL for NTEP-related course content.
- `CADRE_MAPPING_API`: URL for cadre-role mappings (possibly in a health or workforce training context).
- `FRONTEND_URL`: The base URL of your frontend application (e.g., React).
- `BACKEND_URL`: The base URL of your backend API (e.g., NestJS).
- `WATI_AUTH_TOKEN`: Authentication token for WATI (WhatsApp API) used for sending WhatsApp messages.
- `GOOGLE_API_KEY`: Used to access Google APIs like Maps, reCAPTCHA, etc.

## 7. Usage

1. Login with the credentials defined in mongodb
2. Add other admin/supervisor users in Management > Roles & Permissions
3. Setup your master data in Master Tables section
4. Start using Materials, Assessment Creation, Learn Case Findings, Patient Management, Plugin Management etc. modules
5. If you have subscriber app configured, you may see different reports in Reports section

## 8. Contribution Guidelines

Contributions to Ni-Kshay SETU are welcome. If you would like to contribute, please follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b feature/your-feature-name`
3. Make your changes and test thoroughly.
4. Commit your changes: `git commit -m (Format---> feat|fix|docs|style|perf|test : feature or bug fixing description) 
"Add your commit message"`

5. Push to the branch: `git push origin feature/your-feature-name`
6. Create a pull request on the main repository.
7. Provide a clear description of your changes in the pull request.
8. Ensure your code follows the project's coding conventions and style guidelines.
9. Be open to feedback and iterate on your work if requested.

## 9. Test

```bash
# unit tests
$ npm run test
```

## 10.Check swagger API documentation

```bash
# swagger
http://localhost:YOUR_PORT/api/docs
```

## 11. File Structure

<pre>
my-nestjs-app/
│
├── src/
│   ├── app.module.ts
│   ├── app.service.ts
│   ├── app.controller.ts
│   ├── main.ts
│   │
│   ├── common/                # Shared code: interceptors, filters, decorators, etc.
│   │   ├── assets/
│   │   ├── config/
│   │   ├── decorators/
│   │   ├── images/
│   │   ├── mail/
│   │   ├── pagination/
│   │   ├── utils/
│   │   └── watchers/
│   │
│   ├── modules/                # Feature-based modules (domain-driven structure)
│   │   ├── admin-users/
│   │   │   ├── admin-users.module.ts
│   │   │   ├── admin-users.controller.ts
│   │   │   ├── admin-users.service.ts
│   │   │   ├── admin-users.service.spec.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-admin-user.dto.ts
│   │   │   │   ├── login.dto.ts
│   │   │   │   └── update-admin-user.dto.ts
│   │   │   └── entities/
│   │   │       └── admin-user.entity.ts
│   │   │
│   │   ├── subscriber/
│   │   │   ├── subscriber.module.ts
│   │   │   ├── subscriber.controller.ts
│   │   │   ├── subscriber.service.ts
│   │   │   ├── subscriber.service.spec.ts
│   │   │   ├── dto/
│   │   │   │   ├── create-subscriber.dto.ts
│   │   │   │   ├── create-subscriber-v2.dto.ts
│   │   │   │   ├── update-subscriber.dto.ts
│   │   │   │   ├── login.dto.ts
│   │   │   │   ├── otp-generation.dto.ts
│   │   │   │   ├── refresh-token.dto.ts
│   │   │   │   ├── store-device-token.dto.ts
│   │   │   │   └── validate-phoneno.dto.ts
│   │   │   └── entity/
│   │   │       └── subscriber.entity.ts
│   │   │
│   │   ├── feedback/
│   │   ├── leaderboard/
│   │   └── notifications/
│
├── test/                            # Unit & e2e tests
│   ├── auth.service.spec.ts
│   └── app.e2e-spec.ts
│
├── .env                             # Environment variables
├── .env.example                     # Sample env file
├── tsconfig.json
├── nest-cli.json
├── package.json
├── india.topo.json
├── Dockerfile
├── .prettierrc
├── .eslintrc.js
└── README.md
</pre>

## 12. Third Party Documentation

| No. | Service       | Description                                                                        | Documentation Link                                                   |
| --- | ------------- | ---------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| 1   | WATI          | WhatsApp messaging platform for customer communication and automation.             | [WATI API Reference](https://docs.wati.io/reference/introduction)    |
| 2   | SendGrid Mail | Email delivery service used for transactional and marketing emails.                | [SendGrid by Twilio](https://www.twilio.com/docs/sendgrid)           |
| 3   | Firebase      | Admin SDK for Firebase, used for server-side integrations like push notifications. | [firebase-admin (NPM)](https://www.npmjs.com/package/firebase-admin) |
| 4   | TextLocal     | SMS gateway used for sending text messages to users.                               | [TextLocal API Docs](https://api.textlocal.in/docs/)                 |
| 5   | NestJS        | Framework for building efficient and scalable Node.js server-side applications.    | [NestJS Official Docs](https://docs.nestjs.com/)                     |

## 13. License

Ni-Kshay SETU project is licensed under the [GNU General Public License, Version 3.0](https://www.gnu.org/licenses/gpl-3.0).

![Static Badge](https://img.shields.io/badge/Licence-GPL%203.0-blue)
