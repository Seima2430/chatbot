# ???🧑‍💻 Cybersecurity Awareness Bot
youtube link: https://youtu.be/CbRm38lvAS
A simple C# console-based chatbot designed to educate users about basic cybersecurity practices such as password safety, phishing, scams, and safe browsing.

---

## ??👌 Features

- Interactive chatbot conversation
- Personalized user experience (asks for user name)
- Predefined cybersecurity responses
- Input validation and error handling
- Console UI with colors, ASCII art, and typing animation
- Audio greeting on startup

---

## ??? Project Structure

```
CyberSecurityAwarenessBot/
?
??? Program.cs
??? Models/
?   ??? UserProfile.cs
??? Services/
?   ??? AudioPlayer.cs
?   ??? ChatbotService.cs
?   ??? ResponseService.cs
??? UI/
?   ??? ConsoleUI.cs
??? Assets/
    ??? greeting.wav
```

---

## ?? How It Works

### 1. Application Startup
- Displays a styled header using `ConsoleUI`
- Plays a greeting audio (`greeting.wav`)
- Prompts the user to enter their name

### 2. Chat Flow
- The chatbot runs in a loop using `ChatbotService`
- User input is processed by `ResponseService`
- A relevant response is returned based on keywords

### 3. Exit Condition
- Typing `exit` ends the chatbot session

---

## ?? Supported Topics

Users can ask about:

- Password safety  
- Phishing  
- Online scams  
- Suspicious links  
- Safe browsing  
- General chatbot questions (e.g., purpose, capabilities)

---

## ?? Key Components

### ?? Program.cs
- Entry point of the application
- Initializes UI, audio, and chatbot services
- Handles user name input and validation

### ?? UserProfile.cs
- Stores user data (currently only the user's name)

### ?? AudioPlayer.cs
- Plays a `.wav` greeting file at startup
- Handles missing file and playback errors

### ?? ResponseService.cs
- Core logic for chatbot responses
- Uses keyword matching to determine replies

### ?? ChatbotService.cs
- Controls the conversation loop
- Connects user input to chatbot responses

### ?? ConsoleUI.cs
- Handles all console display features:
  - Colored text
  - ASCII banner
  - Typing animation effect
  - Message formatting (bot, user, error, success)

---

## ?? How to Run

### Requirements
- .NET SDK installed (preferably .NET 6 or later)

### Steps

1. Clone or download the project  
2. Open the project in your IDE (Visual Studio recommended)  
3. Ensure the `Assets/greeting.wav` file exists  
4. Run the application:

```
dotnet run
```

---

## ?? Notes & Limitations

- The chatbot uses simple keyword matching (not AI-based)
- Limited understanding of complex or rephrased questions
- Requires `.wav` file format for audio playback
- No persistent user data storage

---

## ?? Possible Improvements

- Replace keyword matching with NLP or AI integration
- Add more cybersecurity topics
- Store chat history or user data
- Improve input parsing (handle typos, synonyms)
- Add a graphical user interface (GUI)

---

## ?? License

This project is for educational purposes. You may modify and use it freely.

---

## ????? Author
* AMAHLE SEIMA *
Developed as a cybersecurity awareness learning project.
