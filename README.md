## Project Structure
    ├── driver
    ├── Jarvis              # Main folder for features 
    │   ├── config          # Contains all secret API Keys
    │   ├── features        # All functionalities of JARVIS 
    │   └── utils           # GUI images
    ├── __init__.py         # Definition of feature's functions
    ├── gui.ui              # GUI file (in .ui format)
    ├── main.py             # main driver program of Jarvis
    ├── requirements.txt    # all dependencies of the program

## Module Imports

In this project, we've imported various libraries to enable different functionalities:

- `JarvisAssistant` module is the core component of our virtual assistant.
- `re` is used for regular expressions, which allows us to process and recognize patterns in user commands.
- `os` provides functions for interacting with the operating system, such as launching applications and managing files.
- `random` helps in generating random responses for greetings.
- `pprint` is used for pretty-printing data structures, making it easier to read and understand complex outputs.
- `datetime` provides functions to work with dates and times, allowing us to provide current time and date information.
- `requests` enables us to make HTTP requests, which is useful for tasks like fetching weather information.
- `sys` provides access to system-specific parameters and functions, allowing us to interact with the system.
- `urllib.parse` is used for parsing URLs, which can be handy for web-related tasks.
- `pyjokes` allows us to generate jokes, adding a touch of humor to our virtual assistant.
- `time` provides various time-related functions, which can be used for adding delays or controlling time-sensitive tasks.
- `pyautogui` gives us control over the mouse and keyboard, enabling automation of various tasks.
- `pywhatkit` is a library for automating tasks related to web services like WhatsApp and YouTube.
- `wolframalpha` allows us to interact with the Wolfram Alpha API for computational intelligence tasks.
- `Image` from the `PIL` library is used for handling images, which is important for tasks like taking screenshots.

## Memory and Constants

We've defined several lists and dictionaries to help our assistant understand and respond to user inputs:

- `GREETINGS` contains various greetings that users might use to initiate interactions with our virtual assistant.
- `GREETINGS_RES` provides corresponding responses to those greetings, making the interaction more natural and engaging.
- `EMAIL_DIC` is a dictionary mapping user-defined email aliases to actual email addresses, facilitating email sending functionality.
- `CALENDAR_STRS` consists of phrases that users might use to inquire about their schedule.

## Function Definitions

### `speak(text)`

This function plays a crucial role in the interaction with the user. It converts text into speech, allowing the assistant to communicate effectively.

### `computational_intelligence(question)`

Here, we interact with the Wolfram Alpha API, sending a user's question and receiving an intelligent response. This adds a layer of computational intelligence to our assistant's capabilities.

## Startup and Wish Functions

- `startup()`: This function handles the initialization process when the assistant is first launched. It checks and calibrates various system components, ensuring everything is in order for a smooth interaction.
- `wish()`: Depending on the time of day, this function greets the user appropriately, setting a friendly tone for the interaction.

Certainly! Here's the continuation of the content:

---

## MainThread Class

The `MainThread` class is pivotal in handling the execution of tasks. It contains the `TaskExecution` method, which is responsible for managing various functionalities based on user input.

### Functionalities

The conditional blocks within the `TaskExecution` method handle a wide range of user commands:

- **Date and Time**: The assistant can provide the current date and time upon user request.

- **Application Launching**: Users can instruct the assistant to launch specific applications, like Google Chrome.

- **Greetings**: The assistant responds to various forms of greetings in a friendly and engaging manner.

- **Website Opening**: Users can ask the assistant to open specific websites.

- **Weather Information**: The assistant fetches and communicates the current weather in a designated city.

- **Information Retrieval**: Users can request information about various topics, which the assistant fetches and communicates.

- **News Headlines**: The assistant provides top headlines from The Times Of India.

- **Google Search**: Users can ask the assistant to perform a Google search.

- **Music Playback**: The assistant can play music from a predefined directory.

- **YouTube Video Playback**: Users can request the assistant to play specific videos on YouTube.

- **Email Sending**: The assistant facilitates email composition and sending based on user instructions.

- **Computational Intelligence**: Users can ask the assistant to perform calculations or provide factual information, which is powered by the Wolfram Alpha API.

- **Location Services**: The assistant can provide information about the location of a specified place.

- **IP Address Retrieval**: The assistant communicates the user's public IP address.

- **Window Switching**: Users can instruct the assistant to switch between open windows.

- **Current Location**: The assistant provides information about the user's current location.

- **Screenshot Capture**: Users can instruct the assistant to take a screenshot, which is then saved with a specified name.

- **Screenshot Display**: The assistant displays the captured screenshot upon user request.

- **File Visibility**: Users can hide or unhide files in the specified directory.

## GUI Initialization

We use PyQt5 to set up the graphical user interface. This includes loading images (such as live wallpaper and initiation animation) and setting up timers for real-time updates.

## Application Startup

The GUI is initiated with the live wallpaper and an initiation animation, creating an engaging start-up experience for the user.

## Application Execution

The application starts the main thread, which handles user commands, and starts the timer for real-time updates.

## Event Handling

Button clicks are handled within the GUI. For example, the "Start" button initiates tasks, while the "Close" button exits the application.

---

This project combines a wide range of functionalities, from basic system interactions to advanced computational intelligence, all wrapped up in an engaging graphical user interface. It provides users with a versatile and user-friendly virtual assistant experience.

1. Greetings:
   - "hello Jarvis"
   - "Jarvis"
   - "wake up Jarvis"
   - "you there Jarvis"
   - "time to work Jarvis"
   - "hey Jarvis"
   - "ok Jarvis"
   - "are you there"

2. Getting Date and Time:
   - "date"
   - "time"

3. Launching Applications:
   - "launch [Application Name]"

4. Opening Websites:
   - "open [Website Name]"

5. Checking Weather:
   - "weather in [City]"

6. Getting Information:
   - "tell me about [Topic]"
   - "what is [Topic]"
   - "who is [Topic]"

7. Reading News:
   - "buzzing"
   - "news"
   - "headlines"

8. Searching on Google:
   - "search google for [Query]"

9. Playing Music:
   - "play music"
   - "hit some music"

10. Playing YouTube Videos:
    - "youtube [Video Name]"

11. Sending Emails:
    - "email"
    - "send email"

12. Calculations:
    - "calculate [Mathematical Expression]"

13. Location Services:
    - "where is [Location]"

14. Getting IP Address:
    - "ip address"

15. Switching Windows:
    - "switch the window"
    - "switch window"

16. Finding Current Location:
    - "where am i"
    - "current location"
    - "where i am"

17. Taking Screenshots:
    - "take screenshot"
    - "take a screenshot"
    - "capture the screen"

18. Displaying Screenshots:
    - "show me the screenshot"

19. Hiding/Showing Files:
    - "hide all files"
    - "hide this folder"
    - "visible"
    - "make files visible"

20. Jokes:
    - "joke"

21. System Information:
    - "system"

22. Exiting Jarvis:
    - "goodbye"
    - "offline"
    - "bye"
