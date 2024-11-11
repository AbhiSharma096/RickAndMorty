# RickAndMorty Application

## Overview

Welcome to the **RickAndMorty Application**! This is a multi-module Android application designed to explore the universe of the popular TV show *Rick and Morty*. The app fetches data about characters, locations, and episodes through a network API. The architecture emphasizes modularity, scalability, and adherence to Android development best practices, including dependency injection and quality coding standards.

## Features

- **Character Listing**: Browse through a complete list of all *Rick and Morty* characters.
- **Character Details**: View detailed information about each character, including their status, origin, and appearances.
- **Locations & Episodes**: Explore different locations and episodes featured in the show.
- **Offline Mode**: The app includes a caching mechanism for offline usage.

## Tech Stack

- **Programming Language**: Kotlin
- **Architecture**: Multi-module architecture for modular development
- **Network Module**: Retrofit for API communication
- **Dependency Injection**: Dagger Hilt for dependency management
- **Data Storage**: Room for caching data locally
- **Image Loading**: Glide for efficient image loading and caching
- **Coroutines**: For asynchronous programming and network calls

## Project Structure

The application follows a multi-module architecture to separate concerns and increase maintainability. Here is a breakdown of the modules:

1. **App Module**: The main module that depends on other feature modules and is responsible for bootstrapping the app.
2. **Network Module**: Contains all the networking code including Retrofit setup, API interface definitions, and network response handling.


## Key Components and Practices

### 1. **Dependency Injection**

The app uses **Dagger Hilt** to manage dependencies, ensuring the code is scalable, testable, and easy to maintain. Hilt is integrated into all modules, providing objects where needed and adhering to *Separation of Concerns*.

### 2. **Network Integration**

- **Retrofit** is used for making HTTP requests to the *Rick and Morty* API.
- **OkHttp** interceptor is used for logging requests and responses, aiding in debugging.
- Error handling mechanisms are implemented to deal with various network states, ensuring that the app provides user-friendly error messages.

### 3. **Multimodule Architecture**

The project follows a multi-module architecture that divides the app into distinct modules such as *network*, *character*, and *episode* modules. This modular approach offers the following benefits:

- **Scalability**: Modules can be developed and maintained independently, making scaling the application easier.
- **Reusability**: Specific modules, such as the *network module*, can be reused across different parts of the application or even in other applications.
- **Encapsulation**: Modules encapsulate specific functionalities, improving the readability and maintainability of the codebase.

### 4. **Coroutines and Flow**

The app uses **Kotlin Coroutines** for handling background tasks, such as making network requests or accessing data from Room. **Flow** is used for observing changes in the data layer, ensuring a reactive approach to UI updates.

### 5. **Offline Caching**

To improve user experience, **Room** is used to store character and episode data locally. When users don't have network access, they can still browse the app with the cached data. The app also synchronizes with the server when the network connection is restored.

## Installation

To run this application, you need to have **Android Studio** installed.

1. Clone the repository from GitHub:
   ```bash
   git clone https://github.com/AbhiSharma096/RickAndMorty.git
   ```

2. Open the project in Android Studio.

3. Sync the project with Gradle to resolve dependencies.

4. Build and run the app on an emulator or physical device.

## API Integration

The app uses the public **Rick and Morty API** (https://rickandmortyapi.com/). Below are some of the key endpoints utilized in the app:

- **Character List**: Fetches a list of all characters from the show.
- **Episode List**: Retrieves a list of episodes, including episode details.
- **Location List**: Provides details on various locations featured in the show.

## Code Quality

The app emphasizes code quality by adhering to the following principles:

- **SOLID Principles**: For maintainable and extendable code.
- **Repository Pattern**: Abstracts the data layer, providing a clean API for accessing data.
- **Clean Architecture**: Separates UI, domain, and data layers for better testability and maintainability.

## Screenshots
<div style="overflow-x: auto; white-space: nowrap;">
  <img src="https://github.com/AbhiSharma096/RickAndMorty/blob/master/ss1.png" width="140">
  <img src="https://github.com/AbhiSharma096/RickAndMorty/blob/master/ss2.png" width="140">
  <img src="https://github.com/AbhiSharma096/RickAndMorty/blob/master/ss3.png" width="140">
  <img src="https://github.com/AbhiSharma096/RickAndMorty/blob/master/ss4.png" width="140">
 
</div>



## Future Improvements

- **Unit Tests**: Increase code coverage with more unit and integration tests.
- **UI Improvements**: Add animations to improve the user experience while navigating through the app.
- **Dark Mode**: Integrate dark mode support for better accessibility.

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Please ensure your code follows the code quality practices defined above.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any inquiries or issues, please contact [Abhishek Sharma](mailto:AbhishekSharma10a@gmail.com).

[GitHub Repository](https://github.com/AbhiSharma096/RickAndMorty.git)

---

Thank you for checking out the **RickAndMorty Application**! Feel free to use the app and contribute to make it better.
