# Todoey

Todoey is a simple yet powerful todo list application built with Flutter. It uses the `provider` package for state management and follows the MVVM (Model-View-ViewModel) architecture.

## Table of Contents

- [Installation](#installation)
- [Features](#features)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)

## Installation

To install and run the Todoey app using Android Studio, follow these steps:

1. **Open Android Studio:**
   Launch Android Studio on your computer.

2. **Clone the Repository:**
   - Go to `File` > `New` > `Project from Version Control...`
   - Select `Git` from the dropdown menu.
   - In the URL field, enter the repository URL: `https://github.com/OswaldSena/todoey_flutter_app.git`
   - Click `Clone`.

3. **Open the Project:**
   After the repository is cloned, Android Studio will automatically open the project.

4. **Install the Dependencies:**
   Open the terminal in Android Studio (bottom-left corner) and run the following command to install the required dependencies:
   ```sh
   flutter pub get
   ```

5. **Run the App:**
   - Connect your Android or iOS device, or start an emulator.
   - Click the `Run` button (green play button) in Android Studio, or run the following command in the terminal:
     ```sh
     flutter run
     ```

## Features

- Add new tasks
- Mark tasks as complete
- Delete tasks
- View the number of tasks
- Persistent state management with `provider`

## Usage

- Launch the app.
- Use the floating action button to add a new task.
- Long-press on a task to delete it.
- Check or uncheck a task to mark it as complete or incomplete.

## File Structure

```
lib
├── main.dart
├── models
│   ├── task.dart
│   └── task_data.dart
├── screens
│   ├── add_task_screen.dart
│   └── tasks_screen.dart
└── widgets
    ├── task_tile.dart
    └── tasks_list.dart
```

- **main.dart**: Entry point of the application. Sets up the `ChangeNotifierProvider`.
- **models/task.dart**: Defines the Task model.
- **models/task_data.dart**: Manages the state of the tasks, including adding, updating, and deleting tasks.
- **screens/add_task_screen.dart**: Screen for adding a new task.
- **screens/tasks_screen.dart**: Main screen displaying the list of tasks.
- **widgets/task_tile.dart**: Represents an individual task item.
- **widgets/tasks_list.dart**: Displays a list of TaskTile widgets.

## Dependencies

- `flutter`
- `provider: ^6.0.0`

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code follows the project's coding standards and includes appropriate tests.

