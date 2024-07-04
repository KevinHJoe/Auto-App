# **Kevin's AutoHotKey Application**

## **Overview**

This application, built using AutoHotKey, is designed to streamline various tasks such as automating order forms, creating forms, and copying names. The application is divided into four main classes: `App`, `Auto-Order-Form`, `Auto-Form-Creator`, and `Auto-Copy-Names`.

## App Class

The `App` class is the main interface of the application. It provides a simple GUI with buttons to navigate to different functionalities. The user can choose between IMP, WRP, and REPS functionalities. Each button hides the main GUI and runs the corresponding script.

## Auto-Order-Form Class

The `Auto-Order-Form` class automates the process of filling out order forms. It performs the following tasks:
- Copies account information from the clipboard.
- Extracts address, city, state, zip, name, phone number, and ID using regular expressions.
- Displays the extracted information in a GUI for user verification.
- Submits the information into an order form, taking into account specific conditions such as the time of day and day of the week.

## Auto-Form-Creator Class

The `Auto-Form-Creator` class assists in creating and managing forms. It:
- Prompts the user to enter their initials if not already provided.
- Allows the user to choose between today's date or a custom date.
- Extracts account information from the clipboard.
- Creates a PDF form using the extracted information and user initials.
- Ensures the PDF is saved to the appropriate location on the user's desktop.

## Auto-Copy-Names Class

The `Auto-Copy-Names` class simplifies the task of copying names from a webpage. It:
- Copies the entire webpage to the clipboard.
- Extracts names from the clipboard using regular expressions.
- Filters out irrelevant text and trims excess characters from the names.
- Provides a GUI with options to print or exit.
- Allows the user to print the extracted names or copy them to the clipboard for further use.

## Usage

1. **Launch the application** by running the main script. A GUI will appear with buttons for IMP, WRP, and REPS.
2. **Choose an option** by clicking on the corresponding button. This will hide the main GUI and run the selected script.
3. **Follow the prompts** provided by the specific script to complete the desired task.

## Dependencies

- AutoHotKey v1.1+
- Word application (for `Auto-Form-Creator` class)

## File Structure

- `App.ahk`: Contains the main GUI and navigation logic.
- `Order.ahk`: Contains the `Auto-Order-Form` class script.
- `Form.ahk`: Contains the `Auto-Form-Creator` class script.
- `Names.ahk`: Contains the `Auto-Copy-Names` class script.

## Notes

- Ensure the working directory is set to the script's location.
- Customize the script icons and GUI appearance as needed.
- Adjust file paths within the script to match your system's directory structure.

