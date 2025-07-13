# Spotify Clone App
A minimal full-stack Spotify clone that allows users to upload and stream their own songs. The application includes secure authentication and a simple music player interface.

This project is built using Flutter for the frontend and Python (FastAPI) for the backend, with PostgreSQL as the database.

## Table of Contents

1. [Introduction](#introduction)  
2. [Features](#features)  
3. [Tech Stack](#tech-stack)  
4. [Project Structure](#project-structure)  
5. [Getting Started](#getting-started)  
   - [Backend Setup](#backend-setup)  
   - [Frontend Setup](#frontend-setup)  
6. [Authentication Flow](#authentication-flow)  
7. [Core Functionality](#core-functionality)  
8. [API Endpoints](#api-endpoints)  
9. [Security](#security)  

 ## Introduction
This project is a simple yet functional Spotify-style music platform. Users can create accounts, upload their songs, and stream them directly from the browser. It’s designed as a learning project that integrates core full-stack development concepts such as authentication, file handling, REST APIs, and frontend-backend communication.

## Features
-User sign-up and login system

-Audio file upload functionality

-Audio streaming

-Auth-protected routes and API endpoints

Clean and responsive user interface built using Flutter Web

## Tech Stack

| Layer      | Technology       | Description                         |
|------------|------------------|-------------------------------------|
| Frontend   | Flutter          | UI framework for building the app   |
|            | Dart             | Programming language for Flutter    |
|            | Audio Player     | Widget for in-browser playback      |
| Backend    | Python           | Core backend language               |
|            | FastAPI          | Web framework for API development   |
|            | JWT              | User authentication and authorization |
| Database   | Postgresql       | Stores user data and song metadata  |

## Project Structure
-client/ — Flutter web frontend

-server/ — Python backend (FastAPI/Flask)

-README.md — Project documentation

-requirements.txt — Backend dependencies

## Getting Started
### Backend Setup
-Create a virtual environment

-Install Python dependencies from the requirements file

-Start the backend server using FastAPI

### Frontend Setup
-Get Flutter packages(pub get)

-Run the app in Chrome or your desired emulator device

## Authentication Flow
-New users can register via the sign-up screen

-Login generates a token (JWT or session-based)

-Authenticated users can upload and stream songs

-Token is stored securely and used in all API requests

## Core Functionality
-Upload songs through a file picker

-View a list of all uploaded songs

-Stream songs via an audio player interface

-Upload and playback are only available to logged-in users

## API Endpoints
### Public Routes

-POST /signup - Register a new user

-POST /login - Authenticate user and return token

### Protected Routes

-POST /upload - Upload audio file

-GET /songs - List all available songs

-GET /stream/{id} - Stream a specific song


## Security
-Passwords are hashed before storing

-Authenticated access is protected via JWT or sessions

-File uploads are restricted to authenticated users

-CORS and content-type headers properly handled
