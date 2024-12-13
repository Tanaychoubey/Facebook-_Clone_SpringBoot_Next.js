# Facebook Clone

## Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Contributing](#contributing)
- [License](#license)

---

## Project Description

This project is a Facebook-like social media platform built using **Next.js** for the frontend and **Spring Boot** with **MySQL** for the backend. It provides essential features for user interaction and content sharing, emulating key functionalities of Facebook.

## Features

### User Features
- **Authentication**: Sign up, log in, and password recovery.
- **Profile Management**: Update profile details, profile picture, and cover photo.
- **Post Management**: Create, edit, delete, like, and comment on posts.
- **Friend System**: Send, accept, and decline friend requests.
- **News Feed**: View posts from friends with real-time updates.
- **Search**: Search for users and pages.
- **Notifications**: Real-time notifications for likes, comments, and friend requests.

### Admin Features
- **User Management**: View and manage user accounts.
- **Content Moderation**: Remove inappropriate posts or comments.

## Technologies Used

- **Frontend**:
  - Next.js
  - Tailwind CSS

- **Backend**:
  - Spring Boot
  - MySQL (Database)

- **Authentication**:
  - JWT (JSON Web Token)

- **Other Tools**:
  - REST APIs
  - Axios (for HTTP requests)

- **Deployment**:
  - Vercel (Frontend)
  - AWS/Heroku (Backend)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Tanaychoubey/facebook-clone-springboot-next.js.git
   cd facebook-clone-springboot-next.js
   ```
2. Install dependencies for both the frontend and backend:
   ```bash
   # Frontend
   cd client
   npm install

   # Backend
   cd ../server
   mvn install
   ```
3. Set up environment variables (see below).
4. Run the application:
   ```bash
   # Backend
   cd server
   mvn spring-boot:run

   # Frontend
   cd ../client
   npm run dev
   ```

## Environment Variables

### Backend (.env or application.properties)

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/facebook-clone-springboot-next.js
spring.datasource.username=your-mysql-username
spring.datasource.password=your-mysql-password
jwt.secret=your-jwt-secret
```

### Frontend (.env.local)

```env
NEXT_PUBLIC_API_BASE_URL=http://localhost:8080
NEXT_PUBLIC_JWT_SECRET=your-jwt-secret
```

## Usage

1. Open the app in your browser at `http://localhost:3000`.
2. Sign up or log in to access the platform.
3. Explore features such as posting, liking, commenting, and managing friends.

## Contributing

Contributions are welcome! To contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m 'Add feature-name'`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
