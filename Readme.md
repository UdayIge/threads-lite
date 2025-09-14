# Threads Lite (Angular + NestJS)

A full-stack light weighted web application that clones the core functionality of Threads, built with Angular for the frontend and NestJS for the backend. This project demonstrates how to build a modern, feature-rich application with a hierarchical commenting system.

This project was created following the tutorial by Mohammad Essan.

-----

## ✨ Features

  * **View a Feed of Threads**: See all top-level posts on the main page.
  * **Create New Threads**: A simple form allows any user to post a new thread.
  * **Nested Replies**: Reply to any thread or comment, creating a hierarchical structure.
  * **Expand/Collapse Comments**: Easily view or hide replies to keep the UI clean.
  * **Persistent User Identity**: The app automatically creates a user identity and saves it in local storage, so you don't need to log in to post.
  * **Fully-Featured Backend**: A robust API built with NestJS to handle all data operations.

-----

## 🛠️ Tech Stack

  * **Frontend**:
      * [Angular](https://angular.io/)
      * [TypeScript](https://www.typescriptlang.org/)
      * [Tailwind CSS](https://tailwindcss.com/)
  * **Backend**:
      * [NestJS](https://nestjs.com/)
      * [TypeScript](https://www.typescriptlang.org/)
  * **Database**:
      * [MongoDB](https://www.mongodb.com/) (using MongoDB Atlas)

-----

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You will need the following software installed on your machine:

  * [Node.js](https://nodejs.org/en/) (v18 or later)
  * [npm](https://www.npmjs.com/) (or yarn)
  * [Git](https://git-scm.com/)
  * A free [MongoDB Atlas](https://www.mongodb.com/cloud/atlas/register) account for the database.

### Installation & Setup

1.  **Clone the repository:**

    ```sh
    git clone https://github.com/your-username/your-repo-name.git
    cd your-repo-name
    ```

2.  **Install Backend Dependencies:**

    ```sh
    cd backend
    npm install
    ```

3.  **Set up Backend Environment Variables:**

      * Create a file named `.env` in the `/backend` directory.
      * Add your MongoDB connection string to this file. You can get this from your MongoDB Atlas dashboard.

    <!-- end list -->

    ```env
    # /backend/.env
    DATABASE_URL=your_mongodb_connection_string_here
    ```

4.  **Install Frontend Dependencies:**

    ```sh
    cd ../frontend
    npm install
    ```

### Running the Application

You'll need to run the backend and frontend servers in two separate terminals.

1.  **Run the Backend Server:**

    ```sh
    # From the /backend directory
    npm run start:dev
    ```

    The NestJS server will be running on `http://localhost:3000`.

2.  **Run the Frontend Development Server:**

    ```sh
    # From the /frontend directory
    ng serve
    ```

    The Angular app will be available at `http://localhost:4200`.

-----

## ☁️ Deployment

This project is configured for easy deployment on **Vercel**. The `vercel.json` file in the root directory handles the build and rewrite rules for this monorepo setup.

To deploy:

1.  Push your code to a GitHub repository.
2.  Import the repository into Vercel.
3.  Add your `DATABASE_URL` as an environment variable in the Vercel project settings.
4.  Deploy\!

-----

## 🙏 Acknowledgements

  * This project was inspired by and built following the excellent tutorial by **Mohammad Essan**.
  * [Link to the original YouTube tutorial](https://www.google.com/search?q=https://youtu.be/cAj6gzAMNfA)