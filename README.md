# 🎬 CineFlow — Movie Streaming Management System

<p align="center">
  <strong>A Web-Based Movie Streaming Management System</strong><br>
  <em>Academic Team Project · Laravel · MySQL</em>
</p>

<p align="center">
  <a href="https://github.com/CaoTHaTrang/CineFlow-Movie-Streaming-Management-System">
    <img src="https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github" alt="GitHub Repository">
  </a>
  <img src="https://img.shields.io/badge/Laravel-Framework-FF2D20?style=for-the-badge&logo=laravel&logoColor=white" alt="Laravel">
  <img src="https://img.shields.io/badge/PHP-8.x-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/MySQL-Database-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL">
  <img src="https://img.shields.io/badge/Bootstrap-UI-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap">
</p>

---

## 📌 Project Overview

**CineFlow** is a web-based **Movie Streaming Management System** developed as an academic team project.

The system is designed to provide an integrated platform for managing and accessing movie-related content through a structured web application. It combines a user-facing movie streaming experience with administrative capabilities for managing movies, categories, users, and other system data.

The project focuses not only on building functional web pages, but also on applying software engineering concepts such as:

* Requirement analysis
* Database design
* CRUD operations
* MVC architecture
* User and administrative workflows
* Search and filtering
* Data validation
* Web application testing
* Version control and collaborative development

> **Project Type:** Academic Team Project
> **Domain:** Entertainment / Movie Streaming
> **Architecture:** MVC
> **Backend:** Laravel / PHP
> **Database:** MySQL
> **Frontend:** Blade, HTML, CSS, JavaScript, Bootstrap

---

# 🎯 Project Objectives

CineFlow was developed to address common management and usability requirements of a movie streaming platform.

### Main objectives

* Build a centralized system for managing movie information.
* Provide users with an intuitive interface for discovering movies.
* Support movie search and filtering.
* Organize movies through categories and related information.
* Provide movie detail pages for users.
* Implement administrative functionality for managing system data.
* Design a structured relational database.
* Apply Laravel MVC architecture to separate application concerns.
* Provide a foundation that can be extended with additional streaming and recommendation features.

---

# 👥 System Users

CineFlow is designed around two primary types of users.

## 👤 Customer / Viewer

Users can interact with the movie platform to:

* Browse available movies.
* Search for movies.
* Filter movie results.
* View movie details.
* Explore movies by category.
* Access movie-related information.
* Interact with the streaming-oriented interface.

## 🔐 Administrator

Administrators are responsible for managing the platform's content and system data.

Typical administrative operations include:

* Manage movies.
* Create, update, and delete movie information.
* Manage movie categories.
* Manage user-related information.
* Maintain system data.
* Monitor and control content displayed on the platform.

---

# ✨ Key Features

## 🎬 Movie Management

The movie management module provides CRUD functionality for maintaining movie information.

Administrators can:

* Add new movies.
* View movie information.
* Update movie details.
* Delete movies.
* Manage movie metadata.
* Associate movies with relevant categories.

---

## 🔎 Search & Filtering

CineFlow provides search and filtering capabilities to improve movie discovery.

Users can:

* Search for movies using keywords.
* Filter movie results.
* Narrow down available content.
* Quickly locate relevant movies.

This functionality improves usability by reducing the amount of manual browsing required to find specific content.

---

## 📖 Movie Details

Each movie can have a dedicated detail page containing relevant information such as:

* Movie title
* Poster / thumbnail
* Description
* Category
* Release-related information
* Movie metadata
* Streaming-related information

The detail page acts as the primary information hub for each movie.

---

## 🏠 Homepage

The homepage provides an entry point into the CineFlow platform.

It is designed to help users:

* Discover available movies.
* Navigate to different sections.
* Access movie categories.
* Find featured or relevant content.
* Quickly navigate to movie detail pages.

---

## 🗂️ Category Management

Movies can be organized into categories to improve content discovery and administration.

The category management functionality supports:

* Creating categories.
* Updating categories.
* Removing categories.
* Associating movies with categories.
* Organizing movie content systematically.

---

## 👨‍💼 Administrative Management

The administration area provides centralized control over the application's content.

The administrator can manage core system entities through dedicated management interfaces rather than directly modifying database records.

This helps maintain:

* Data consistency
* Operational efficiency
* Structured workflows
* Easier content maintenance

---

# 🏗️ System Architecture

CineFlow follows the **Model–View–Controller (MVC)** architectural pattern provided by Laravel.

```text
                    ┌─────────────────────┐
                    │       User          │
                    │ Customer / Admin    │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │       Routes        │
                    │   HTTP Requests     │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Controllers      │
                    │ Business Logic      │
                    └───────┬─────┬───────┘
                            │     │
                 ┌──────────┘     └──────────┐
                 ▼                           ▼
        ┌─────────────────┐         ┌─────────────────┐
        │     Models      │         │      Views      │
        │  Data / ORM     │         │ Blade / UI      │
        └────────┬────────┘         └─────────────────┘
                 │
                 ▼
        ┌─────────────────┐
        │     MySQL       │
        │    Database     │
        └─────────────────┘
```

### Architecture responsibilities

| Layer           | Responsibility                                    |
| --------------- | ------------------------------------------------- |
| **Routes**      | Defines application endpoints and request routing |
| **Controllers** | Handles requests and application logic            |
| **Models**      | Represents database entities and relationships    |
| **Views**       | Provides user-facing interfaces using Blade       |
| **Database**    | Stores persistent application data                |
| **Middleware**  | Handles request filtering and access control      |

---

# 🗄️ Database Design

The application uses a relational database to manage structured movie streaming data.

The database is designed to support relationships between core entities such as:

```text
Users
   │
   ├── User Information
   │
   └── Authentication / Access

Movies
   │
   ├── Movie Information
   ├── Category
   └── Streaming-related Data

Categories
   │
   └── Movie Classification
```

The Laravel migration system is used to define and manage database structures in a version-controlled manner.

### Database considerations

The database design focuses on:

* Data integrity
* Entity relationships
* Primary and foreign keys
* Consistent data types
* Maintainability
* Scalability
* Separation between application logic and persistent data

---

# 🧩 Technology Stack

## Backend

* **PHP**
* **Laravel**
* Laravel MVC
* Laravel Eloquent ORM
* Laravel Routing
* Laravel Middleware
* Laravel Blade

## Frontend

* HTML5
* CSS3
* JavaScript
* Bootstrap
* Blade Templates

## Database

* MySQL
* Laravel Migrations
* Eloquent ORM

## Development Tools

* Git
* GitHub
* Visual Studio Code
* Composer
* Node.js / npm
* XAMPP / local PHP development environment

---

# 📁 Project Structure

The project follows Laravel's standard application structure.

```text
CineFlow-Movie-Streaming-Management-System/
│
├── app/
│   ├── Http/
│   │   ├── Controllers/
│   │   └── Middleware/
│   └── Models/
│
├── bootstrap/
│
├── config/
│
├── database/
│   ├── migrations/
│   ├── seeders/
│   └── factories/
│
├── public/
│   ├── css/
│   ├── js/
│   └── images/
│
├── resources/
│   └── views/
│       ├── layouts/
│       ├── admin/
│       └── ...
│
├── routes/
│   ├── web.php
│   └── ...
│
├── storage/
│
├── tests/
│
├── .env.example
├── artisan
├── composer.json
└── package.json
```

---

# 🔄 Core Application Workflow

A simplified movie browsing workflow is:

```text
User
 │
 ▼
Homepage
 │
 ├───────────────┐
 ▼               ▼
Search         Category
 │               │
 └───────┬───────┘
         ▼
   Movie Listing
         │
         ▼
   Movie Details
         │
         ▼
 Streaming Experience
```

The administrative workflow follows:

```text
Administrator
      │
      ▼
 Admin Dashboard
      │
      ├── Movie Management
      │       ├── Create
      │       ├── Read
      │       ├── Update
      │       └── Delete
      │
      ├── Category Management
      │
      └── User / System Management
```

---

# 🧪 Testing & Quality Assurance

Testing is an important part of the development process.

The system can be evaluated through different testing scenarios, including:

### Functional Testing

* Verify movie creation.
* Verify movie editing.
* Verify movie deletion.
* Verify movie searching.
* Verify movie filtering.
* Verify movie detail navigation.
* Verify category operations.
* Verify administrator workflows.

### Validation Testing

* Required field validation.
* Invalid input handling.
* Duplicate data handling.
* Boundary-value validation.
* Form submission validation.

### UI Testing

* Navigation consistency.
* Layout responsiveness.
* Button functionality.
* Form usability.
* Movie listing presentation.
* Detail page presentation.

### Regression Testing

After implementing new features or fixing defects, previously implemented functionality should be retested to ensure that existing features remain stable.

---

# 🔐 Security Considerations

The project follows common web application security practices provided by Laravel.

Key considerations include:

* Environment variables stored in `.env`.
* `.env` excluded from version control.
* `.env.example` provided for configuration reference.
* Server-side validation.
* Authentication and authorization mechanisms.
* CSRF protection.
* Secure database interaction through Laravel's ORM/query mechanisms.
* Separation of configuration from application source code.

> **Important:** Never commit `.env`, database passwords, API keys, or other secrets to a public repository.

---

# 🚀 Installation & Setup

## 1. Clone the repository

```bash
git clone https://github.com/CaoTHaTrang/CineFlow-Movie-Streaming-Management-System.git
```

```bash
cd CineFlow-Movie-Streaming-Management-System
```

---

## 2. Install PHP dependencies

```bash
composer install
```

---

## 3. Install frontend dependencies

```bash
npm install
```

---

## 4. Create environment configuration

Copy the example environment file:

```bash
cp .env.example .env
```

On Windows CMD:

```cmd
copy .env.example .env
```

---

## 5. Generate application key

```bash
php artisan key:generate
```

---

## 6. Configure the database

Open `.env` and configure the local database:

```env
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=cineflow
DB_USERNAME=root
DB_PASSWORD=
```

> Adjust the database name, username, and password according to your local environment.

---

## 7. Run migrations

```bash
php artisan migrate
```

If seeders are available:

```bash
php artisan db:seed
```

or:

```bash
php artisan migrate --seed
```

---

## 8. Create storage link

```bash
php artisan storage:link
```

---

## 9. Start the Laravel development server

```bash
php artisan serve
```

The application will normally be available at:

```text
http://127.0.0.1:8000
```

---

# 🖥️ Screenshots

> Screenshots can be added here to demonstrate the main system interfaces.

### Homepage

![CineFlow Homepage](screenshots/homepage.png)

### Movie Listing

![Movie Listing](screenshots/movie-listing.png)

### Movie Details

![Movie Details](screenshots/movie-details.png)

### Admin Dashboard

![Admin Dashboard](screenshots/admin-dashboard.png)

### Movie Management

![Movie Management](screenshots/movie-management.png)

> **Note:** Replace the image paths above with the actual screenshots included in the repository.

---

# 👩‍💻 My Contributions

CineFlow was developed as a **team-based academic project**. My contribution focused on selected parts of the system rather than representing the work of the entire team.

### Areas of contribution

* Participated in requirement analysis and system discussion.
* Contributed to system design and feature planning.
* Worked on movie management functionality.
* Contributed to movie search and filtering functionality.
* Worked with Laravel MVC architecture.
* Participated in database-related implementation.
* Contributed to UI implementation and refinement.
* Performed functional testing and debugging.
* Used Git/GitHub for version control and collaborative development.

> **Note:** This section should be customized to accurately reflect the specific features and tasks completed by each team member.

---

# 📚 Academic Context

This project was developed as part of an academic web development project.

The project provided practical experience in:

* Web application development
* Requirements analysis
* Database management
* MVC architecture
* CRUD implementation
* Software testing
* Debugging
* Git version control
* Collaborative software development

It also provided an opportunity to connect theoretical knowledge with a real-world-style information system.

---

# 🔮 Future Improvements

Potential future enhancements for CineFlow include:

### 🎞️ Advanced Streaming

* Video streaming integration.
* Multiple video qualities.
* Subtitle support.
* Continue-watching functionality.
* Watch history.

### ⭐ User Experience

* Movie ratings and reviews.
* Favorites / watchlist.
* Personalized recommendations.
* Recently watched movies.
* Advanced search.

### 🤖 Recommendation System

A recommendation engine could be introduced using:

* Content-based filtering.
* Collaborative filtering.
* Hybrid recommendation.
* User preference analysis.

### 📊 Administration & Analytics

* User activity dashboard.
* Movie popularity statistics.
* Streaming analytics.
* Category performance.
* User engagement reports.

### ☁️ Deployment

The system can be further prepared for deployment using:

* Production database.
* Cloud hosting.
* CI/CD pipeline.
* Environment-specific configuration.
* Application monitoring.

---

# 📈 Project Learning Outcomes

Through the development of CineFlow, the project team gained practical experience in the complete software development workflow:

```text
Requirements
     ↓
System Analysis
     ↓
Database Design
     ↓
UI / UX Design
     ↓
Implementation
     ↓
Testing
     ↓
Debugging
     ↓
Version Control
     ↓
Deployment Preparation
```

The project strengthened understanding of how different components of an information system work together, from user requirements and database design to backend processing and frontend interaction.

---

# 📝 Project Status

**Current Status:** Completed Academic Project

The current repository contains the implemented source code and development history of the CineFlow Movie Streaming Management System.

Further improvements can be introduced as future iterations of the project.

---

# 👥 Team Project

CineFlow was originally developed collaboratively by a team of students.

This repository represents a personal copy of the academic project maintained for:

* Portfolio documentation
* Technical reference
* Project demonstration
* Continued development
* Academic showcase

All team contributions should be appropriately acknowledged when presenting the project publicly.

---

# 📄 License

This project was created for academic and educational purposes.

If the original team project has specific licensing or university requirements, those requirements should take precedence over this section.

---

# 📬 Contact

**Cao Thi Ha Trang**

Management Information Systems Student

GitHub:
https://github.com/CaoTHaTrang

Portfolio:
https://caothatrang.github.io/Portfolio-/

Email:
[caohatrang0069@gmail.com](mailto:caohatrang0069@gmail.com)

---

<p align="center">
  <strong>🎬 CineFlow — Discover. Stream. Experience.</strong>
</p>

<p align="center">
  <em>Movie Streaming Management System</em>
</p>
