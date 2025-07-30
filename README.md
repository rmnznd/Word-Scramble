Word-Scramble
A fun and challenging word game built with SwiftUI, where players form new words from a given root word. Test your vocabulary and spelling skills!

🎮 How to Play
Start the Game: When you launch the app, a random 8-character word will appear at the top of the screen. This is your root word.

Enter Your Word: In the text field, type a word that can be formed using only the letters from the root word.

Submit: Press the "Return" key on your keyboard to submit your word.

Validity Checks:

Originality: You cannot use the same word twice.

Possibility: All letters in your submitted word must come from the root word, and you cannot use any letter more times than it appears in the root word.

Real Word: The game checks if your word is a valid English word using a built-in spell checker.

Feedback:

Correct Word: If your word is valid, it will be added to a list below the input field, along with its letter count.

Incorrect Word: If your word is invalid, an alert will pop up explaining why (e.g., "Word used already," "Word not possible," or "Word not recognized"). Dismiss the alert and try again!

Continue Playing: Keep finding and submitting words until you've exhausted all possibilities or want to restart the app for a new challenge.

✨ Features
Dynamic Root Word: A new 8-character word is randomly selected from a large dictionary file (start.txt) each time the game starts.

Input Validation:

Prevents duplicate word entries.

Ensures words are formed only from the letters of the root word.

Validates words against a dictionary for correctness.

User-Friendly Interface: Clean and intuitive design using SwiftUI's List and NavigationStack.

Visual Feedback: Displays submitted words with their letter count.

Error Alerts: Provides clear messages for invalid word submissions.

🛠️ Requirements
Xcode: Version 15.0 or later

iOS: 17.0 or later

Swift: 5.9 or later

start.txt file: A text file containing a list of words (one word per line) must be included in the project bundle. The current implementation expects this file to contain at least 9,000 different words.

🚀 Installation & Setup
Clone the Repository:

git clone https://github.com/YOUR_USERNAME/Word-Scramble.git

Navigate to the Project Directory:

cd Word-Scramble

Open in Xcode:
Open the Word-Scramble.xcodeproj file in Xcode.

Add start.txt:

Ensure you have a start.txt file in your project's main bundle. This file should contain a list of words, each on a new line.

If you don't have one, create a new file named start.txt in Xcode (File > New > File... > Empty) and make sure it's added to your target's "Copy Bundle Resources" in the "Build Phases" tab.

Run the App:
Select a simulator or a physical device and click the "Run" button (▶️) in Xcode.

📂 Project Structure
ContentView.swift: Contains the main SwiftUI view logic, including game state management, UI layout, and core game functions (addNewWord, startGame, isOriginal, isPossible, isReal, wordError).

start.txt: (Expected in project bundle) A plain text file containing the dictionary of words used for the root word selection.

💡 Future Enhancements
Score Tracking: Implement a scoring system based on word length or difficulty.

Restart Button: Add a button to easily restart the game with a new root word without relaunching the app.

Minimum Word Length: Introduce a configurable minimum length for valid submitted words.

Timer: Add a timer for timed gameplay challenges.

Difficulty Levels: Allow users to choose different root word lengths or word list sizes.

Haptic Feedback: Provide subtle haptic feedback for correct/incorrect submissions.

📄 License
This project is open-source and available under the MIT License.

✍️ Author
Ramin Zand
