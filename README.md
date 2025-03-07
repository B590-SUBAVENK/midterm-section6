# Android Notes App

This project is a straightforward note-taking application that allows authenticated users to create, view, update, and remove notes, with Firebase providing secure login functionality.

## Overview

The application integrates Firebase Authentication for user logins, coupled with a local database for storing note data. It presents a login interface, a main screen displaying all notes in a RecyclerView, and a separate screen for editing individual notes. Users can compose new notes, modify existing ones, and remove notes after a confirmation prompt.

## Key Features

- **User Authentication**: Secure login handling is powered by Firebase Authentication.
- **Notes Display**: A RecyclerView presents notes in a scrollable list.
- **Note Creation**: Users can add entries with both title and description.
- **Note Modification**: Existing notes can be edited directly in an editing interface.
- **Note Removal**: Users can remove notes with a simple confirmation dialog.
- **Local Data Management**: Room Database ensures data persistence on the device.

## Additional Enhancements

- **Material Design**: UI elements follow Material guidelines for a clean user experience.
- **Efficient Database Usage**: Background threads are used to handle data operations, preventing UI freezes.
- **User-Friendly Animations**: Animated transitions create a smoother workflow.
- **Validation Checks**: Empty or invalid inputs are blocked to maintain data integrity.
- **Automatic Time Stamps**: Each note is tagged with its creation or modification time.

## Demonstration

Below is a short recording showing the main user paths:

![Video Walkthrough](WalkThrough.gif)

During the walkthrough, you will see:
- User login
- Creating new notes
- Editing existing notes
- Deleting notes after a confirmation
- Navigating between screens
- Data remaining intact after app restarts

## Remarks

- The login screen is connected to Firebase for credential verification.
- All database interactions run off the main thread to keep the UI responsive.
- The app adopts the MVVM pattern to separate data handling, UI, and logic.
- RecyclerView efficiently reuses views to enhance scrolling performance.
- DialogFragment is employed to confirm note deletion in accordance with Android UI best practices.

## License

This software is distributed under the MIT License. See the [LICENSE](LICENSE) file for further details.