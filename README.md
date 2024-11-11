# RickAndMorty Application

A multi-module Android application featuring data from the Rick and Morty universe. This project implements a clean architecture with a focus on maintainable, scalable, and testable code, using modularization, network handling, dependency injection, and quality code practices.

## Table of Contents
- [Features](#features)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## Features
- **Character Search:** Browse through Rick and Morty characters with detailed information.
- **Multi-Module Architecture:** Separation of concerns with dedicated modules for networking, UI, and data.
- **Offline Caching:** View previously loaded data without an internet connection.
- **Dependency Injection:** Managed dependencies using Dagger Hilt.
- **High Code Quality Standards:** SOLID principles, Repository pattern, and other best practices for maintainable code.

## Architecture
The project follows a **multi-module Clean Architecture** to achieve better code organization, separation of concerns, and scalability. Here’s a quick overview:

1. **UI Module:** Handles user interactions and displays data using Jetpack Compose.
2. **Data Module:** Manages data from different sources such as remote APIs and local caching.
3. **Network Module:** Handles all network calls to the Rick and Morty API.
4. **Domain Module (Future Plan):** Serves as an intermediary between UI and Data modules, handling business logic (currently part of the data module).

## Technologies Used
- **Kotlin** - Primary language for Android development.
- **Dagger Hilt** - Dependency Injection.
- **Retrofit** - For network requests.
- **OkHttp** - HTTP client for handling requests and logging.
- **Jetpack Compose** - Modern UI toolkit for Android.
- **Room Database** - Local data storage for offline caching.
- **Coroutines** - For asynchronous tasks and smooth UI.
- **SOLID Principles** - For high-quality, maintainable code.
- **Rick and Morty API** - The primary API source for character data.

## Project Structure
The app is modularized to separate responsibilities:
