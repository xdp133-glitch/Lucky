# Lucky - Project Generator & Mini-IDE

An application to generate, manage, and edit projects, with a powerful suite of tools for developers, including a Monaco-based code editor, live web preview, and integrated SSH for remote deployment.

## About The Project

`lucky` is a Flutter application designed to be a lightweight, mobile-first development environment. It streamlines the creation of new projects using templates and provides a robust set of tools to manage the entire development and deployment workflow from a single app.

At its core, `lucky` combines a powerful code editor with seamless remote server management, making it an ideal tool for web development on the go.

## Features

### 🚀 Integrated Development Environment

*   **Monaco-Powered Code Editor**: Enjoy a rich editing experience based on the same engine as VS Code, running within the app. Features include:
    *   Syntax highlighting for numerous languages.
    *   Command Palette for advanced actions.
    *   Search and Replace functionality.
    *   Code formatting, Undo/Redo, and more.
*   **Tabbed Interface**: Open and manage multiple files simultaneously in a clean, tabbed layout. The editor will prompt you to save unsaved changes before closing a tab.
*   **Customizable Experience**: A dedicated settings panel allows you to personalize the editor with options for font size, word wrap, minimap visibility, and more.
*   **File Explorer**: A built-in file explorer to browse, open, create, rename, and delete files and folders within your project.

### 🌐 Web Development & Live Preview

*   **Live Web Server**: The app runs a local HTTP server to serve your web project files.
*   **Real-time Preview Panel**: Instantly see your changes in a live preview panel rendered in a separate webview. 
*   **Device Simulation**: Toggle between different device formats (e.g., Mobile, Desktop) to test the responsiveness of your web projects.
*   **Automatic Web Project Detection**: The app automatically scans your project to find valid web project folders (containing `.html`, `.css`, `.js`) to serve for the preview.

### 🛰️ Advanced SSH & Remote Management

*   **Automatic Remote Upload on Save**: When a file is saved, it is automatically and seamlessly uploaded to your configured remote server via SSH, creating an efficient "save-and-deploy" workflow.
*   **Full SSH Configuration**: A dedicated settings page to manage all your connection details, with support for both **password** and **private key** authentication.
*   **Multi-Tab Terminal**: Manage multiple SSH sessions in a tabbed terminal interface powered by `Xterm`. Includes a **Favorite Commands Palette** to save and quickly execute your most-used shell commands.

### 🗂️ Template-Based Project Generation

*   **Scaffold New Projects**: Quickly generate new projects from a catalog of templates defined in `.md` files.
*   **Markdown-Defined Structure**: Templates use a YAML front matter for metadata and a Markdown body to define the folder and file structure.
*   **Categorization & Preview**: Templates are organized by category, and you can preview the project structure before generation.

## Getting Started

### Prerequisites

- Flutter SDK installed on your machine.

### Installation

1.  Clone the repo: `git clone https://github.com/your_username/flutter_folder_creator.git`
2.  Navigate to the directory: `cd flutter_folder_creator`
3.  Install dependencies: `flutter pub get`
4.  Run the app: `flutter run`

## Workflow Example

1.  **Configure SSH**: Go to the **SSH Settings** page to enter your server credentials. Test and save your configuration.
2.  **Generate a Project**: Navigate to the **Templates** section and generate a new web project.
3.  **Start Editing**: The project opens in the **Editor**. Open an HTML file.
4.  **Live Preview**: Toggle the preview panel to see your website render as you type.
5.  **Save & Deploy**: Save the file. The changes are automatically uploaded to your server.
6.  **Manage Server**: Switch to the **Terminal** page to run commands on your remote server, like restarting a service.

## Project Structure

*   `lib/`: Core Dart source code.
    *   `screens/`: UI for each major feature (Editor, Terminal, Templates, etc.).
    *   `services/`: Business logic (SSH, Terminal Management, Local Server, etc.).
    *   `notifiers/`: State management.
*   `assets/`: Static assets.
    *   `templates_catalog/`: Project templates.
    *   `monaco/`: Assets for the Monaco web editor.

You can download the release now, and feel free to share your feedback! 😄

