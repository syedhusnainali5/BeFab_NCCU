# BeFAB-NCCU

<p align="center">
  <strong>Be Fit, Active, & Balanced</strong><br/>
  A Digital Health, Fitness, Nutrition & Wellness Platform
</p>

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.befab.fitness">
    <img src="https://img.shields.io/badge/Google_Play-Download-34A853?style=for-the-badge&logo=googleplay&logoColor=white" alt="Google Play"/>
  </a>
  <img src="https://img.shields.io/badge/Framework-Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter"/>
  <img src="https://img.shields.io/badge/Language-Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white" alt="Dart"/>
</p>

---

## ⚠️ Important Repository Notice

**This repository contains Flutter boilerplate/starter code and is NOT the actual BeFAB-NCCU production application.**

The original BeFAB-NCCU platform is a fully developed digital wellness solution with a mobile application, backend services, database operations, and an administrative management system.

This repository is intended to provide a Flutter development starting point and a technical overview of the actual BeFAB-NCCU product.

It does not contain the complete production application, its proprietary business logic, production backend, database, administrative dashboard, credentials, or private infrastructure.

For the actual application, please visit the official Google Play listing:

**[Download BeFAB-NCCU on Google Play](https://play.google.com/store/apps/details?id=com.befab.fitness)**

---

## 1. About BeFAB-NCCU

**BeFAB (Be Fit, Active, & Balanced)** is a digital health, fitness, nutrition, and wellness platform developed for the North Carolina Central University (NCCU) community.

The platform aims to encourage healthier lifestyles through digital wellness tracking, personalized goals, educational resources, community engagement, fitness activities, nutrition management, and research-enabled surveys.

It provides a centralized digital environment where students, faculty, and other participating community members can monitor their wellness journeys, participate in challenges, access educational materials, and engage with research-oriented activities.

The platform emphasizes:

- Health and fitness awareness.
- Nutrition and hydration management.
- Personalized wellness goals.
- Physical activity tracking.
- Community engagement.
- Educational resources.
- Research-enabled surveys and feedback.
- User privacy and secure data handling.

## 2. Application Features

The production BeFAB-NCCU application includes several integrated modules.

### 📊 Personalized Health Dashboard

Users can access a customizable dashboard containing important wellness information.

Features include:
- Daily activity overview.
- Personal fitness goals.
- Nutrition tracking.
- Hydration monitoring.
- Sleep information.
- Wellness progress.
- Customizable dashboard cards.

### 🏃 Fitness & Activity Tracking

Users can monitor physical activities and fitness progress.

Features include:
- Daily movement tracking.
- Workout information.
- Activity monitoring.
- Heart rate information where supported.
- Manual activity data entry.
- Fitness progress visualization.

### 🎯 Goals & Progress Management

The application allows users to establish personalized health and fitness objectives.

Features include:
- Custom goal creation.
- Progress monitoring.
- Milestone tracking.
- Personalized suggestions.
- Goal reminders.
- Performance insights.

### 🥗 Nutrition & Meal Tracking

The nutrition module helps users monitor their dietary habits.

Features include:
- Meal logging.
- Food database search.
- Barcode-based food scanning.
- Nutrition information.
- Dietary tracking.
- Daily hydration management.
- Water intake reminders.

### 👥 Community, Groups & Competitions

BeFAB provides community-oriented engagement features.

Features include:
- Community groups.
- Fitness challenges.
- Research-driven activities.
- Leaderboards.
- Achievement sharing.
- Competition participation.
- Community interaction.

Privacy is an important consideration: usernames are used as public identifiers rather than exposing users' real names or profile photographs.

### 🎬 Video & Educational Resources

The platform provides a resource library for wellness education and engagement.

Features include:
- Wellness videos and reels.
- Educational materials.
- Community resources.
- Admin-published content.
- Resource discovery.
- Video-based learning.

### 📝 Surveys & Research

Research-enabled surveys provide a way to collect participant feedback and support research-oriented activities.

Features include:
- Survey availability.
- Research-related questionnaires.
- Class-based surveys.
- Participant feedback.
- Survey participation management.
- Structured response collection.

Participation and consent are important considerations in the research workflow.

### 🔐 Privacy & User Support

The application incorporates privacy-focused functionality.

Features include:
- Privacy information.
- Terms and agreements.
- User support access.
- Secure data transmission.
- Privacy-conscious community interactions.
- User data rights information.

---

## 3. Administrative Management System

BeFAB is not simply a standalone mobile application. It operates alongside a centralized administrative management system.

The administrative system provides authorized administrators with the ability to manage the platform, its users, content, programs, and activities.

### Administrative Responsibilities

**1. User Management**
- View registered users.
- Access relevant user information.
- Manage user-related records.
- Support platform administration.

**2. Programs & Activities**
- Manage wellness programs.
- Organize activities and initiatives.
- Coordinate community participation.
- Maintain program-related information.

**3. Content Management**
- Manage educational resources.
- Publish wellness content.
- Maintain video and resource libraries.
- Update information presented within the application.

**4. Surveys & Research Management**
- Manage research-oriented survey activities.
- Organize questionnaires.
- Review collected responses through authorized workflows.
- Support research-related data management.

**5. Platform Administration**
- Manage administrative operations.
- Maintain application content and information.
- Coordinate user support.
- Oversee platform activities.

### How the Administration System Works

The overall workflow can be understood as follows:

1. An authorized administrator accesses the administrative dashboard.
2. The dashboard communicates with the backend through authenticated API requests.
3. The backend validates the administrator's permissions.
4. Authorized operations are performed against the relevant database records.
5. Updated information is returned to the administrative dashboard.
6. Where applicable, changes become available to users through the mobile application.
7. The mobile application retrieves updated information through the backend APIs.

### Administrative Architecture

```text
           ADMINISTRATOR
                 |
                 v
       ADMINISTRATIVE DASHBOARD
                 |
                 v
          BACKEND REST APIs
                 |
          Authentication
          Authorization
          Validation
                 |
                 v
              DATABASE
                 |
          +------+------+
          |             |
          v             v
      User Data     Platform Data
          |             |
          +------+------+
                 |
                 v
         MOBILE APPLICATION
                 |
                 v
             END USERS
```

The administrative dashboard and Flutter application are separate client interfaces that interact with the backend services.

**Important:** The diagram describes the production platform's conceptual architecture. The actual administrative dashboard, backend implementation, database, and production integrations are not included in this Flutter boilerplate repository.

---

## 4. High-Level Technical Architecture

The production platform follows a client-server architecture.

| Component | Responsibility |
|---|---|
| Flutter Mobile App | User-facing mobile experience |
| Backend Services | Business logic and API processing |
| REST APIs | Communication between application and backend |
| Database | Persistent storage and data management |
| Admin Dashboard | Administrative operations and management |
| Authentication | User identity and access control |

### Application Communication Flow

The mobile application communicates with backend services through REST APIs.

Typical operations include:

- Authentication and account operations.
- Retrieving dashboard information.
- Submitting fitness and wellness data.
- Managing personal goals.
- Recording meals and hydration.
- Retrieving community information.
- Accessing educational resources.
- Submitting survey responses.

The backend processes requests, validates data, applies authorization rules, interacts with the database, and returns appropriate responses.

---

## 5. Repository Scope

This repository is intentionally limited to Flutter boilerplate code.

| Included | Not Included |
|---|---|
| Flutter starter structure | Actual production mobile application |
| Boilerplate Dart code | Production business logic |
| Basic application scaffolding | Production backend |
| Development starting point | Production database |
| Project documentation | Admin dashboard |
| Flutter configuration | Production credentials |
| Starter dependencies | Private infrastructure |

This distinction is important when exploring the repository or using it as a reference for development.

---

## 6. Getting Started

### Prerequisites

Install the following development tools:

- Flutter SDK
- Dart SDK
- Android Studio or Visual Studio Code
- Android SDK
- Git

Verify your Flutter installation:

```bash
flutter doctor
```

### Clone the Repository

```bash
git clone <REPOSITORY_URL>
```

Navigate into the project:

```bash
cd <PROJECT_DIRECTORY>
```

Install dependencies:

```bash
flutter pub get
```

Run the application:

```bash
flutter run
```

Build an Android APK:

```bash
flutter build apk --release
```

Build an Android App Bundle:

```bash
flutter build appbundle --release
```

**Note:** These commands apply to the Flutter starter project. They do not build or reproduce the production BeFAB-NCCU application.

---

## 7. Production Application

The actual BeFAB-NCCU application is publicly available on Google Play.

<p align="center">
  <a href="https://play.google.com/store/apps/details?id=com.befab.fitness">
    <strong>BeFAB-NCCU — Google Play Store</strong>
  </a>
</p>

**Application name:** BeFAB-NCCU  
**Full name:** Be Fit, Active, & Balanced  
**Platform:** Android/iOS  
**Application category:** Health & Fitness

The application is designed for a research-oriented wellness community and combines health tracking, nutrition, physical activity, social engagement, educational content, and research-enabled participation.

---

## 8. Important Notes for Developers

Before working with this repository, please understand:

1. This is not a source-code release of the actual BeFAB-NCCU application.
2. The production application's complete Flutter implementation is not available here.
3. The backend and administrative system are separate components.
4. Production API endpoints and credentials are not provided.
5. Features described in this README belong to the actual BeFAB-NCCU product, not necessarily to the boilerplate code.
6. Reproducing the production platform requires implementing the relevant mobile, backend, database, and administrative components independently.

---

## 9. Project Purpose

The purpose of this repository is to provide a starting point for Flutter development while documenting the broader BeFAB-NCCU ecosystem.

It helps developers understand the product's objectives, functionality, user experience, administrative workflows, and high-level technical architecture without misrepresenting this repository as the original production source code.

---

## 10. References

- **Official Android Application:** [BeFAB-NCCU on Google Play](https://play.google.com/store/apps/details?id=com.befab.fitness)
- **North Carolina Central University:** [NCCU Official Website](https://www.nccu.edu/)
- **Flutter Documentation:** [flutter.dev](https://flutter.dev/)
- **Dart Documentation:** [dart.dev](https://dart.dev/)

---

<p align="center">
  <strong>BeFAB — Be Fit, Active, & Balanced</strong><br/>
  Empowering research-based wellness: track, share, and thrive.
</p>
