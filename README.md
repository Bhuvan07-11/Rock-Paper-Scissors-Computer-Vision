# ✋ Rock Paper Scissors – Computer Vision Edition

Play the classic Rock-Paper-Scissors game using just your **webcam and hand gestures**! This project uses computer vision and hand-tracking to detect your finger positions in real time and compete against an AI opponent.

## 🎮 Demo

<img width="1598" height="932" alt="Screenshot 2026-06-14 023821" src="https://github.com/user-attachments/assets/945fcf8f-ebd4-4d33-a1ba-e2dd770df3ab" />
<img width="1600" height="937" alt="Screenshot 2026-06-14 023842" src="https://github.com/user-attachments/assets/9d7e71ec-8157-4db6-b184-de1570e101c4" />
<img width="1598" height="937" alt="Screenshot 2026-06-14 023941" src="https://github.com/user-attachments/assets/1b8cc9f5-b184-4f20-98df-e066af877254" />

## 🚀 Features

- Real-time hand detection and finger tracking with on-screen landmarks
- Gesture classification into Rock, Paper, or Scissors
- 3-second countdown before each round
- AI randomly selects its move
- Live score tracking for AI vs Player
- Clean, colorful UI built with OpenCV overlays

## 🛠️ Tech Stack

- **Python**
- **OpenCV** – for video capture, image processing, and UI rendering
- **MediaPipe** – for hand landmark detection and tracking
- **NumPy** – for numerical operations
- **Random** – for AI move generation

## 📦 Installation

1. Clone the repository
```bash
git clone https://github.com/your-username/ROCK-paper-Scissor.git
cd ROCK-paper-Scissor
```

2. Install dependencies
opencv-python
mediapipe
numpy

## ▶️ Usage

Run the main script:
```bash
python main.py
```

## 🎮 How to Play

1. Focus on the game window and press the **`s`** key on your keyboard to start a round.
2. A countdown from **3** will appear in the middle of the screen.
3. Show one of the following gestures to your webcam before the countdown ends:
   - ✊ **Rock** – Fist (all fingers down)
   - 🖐️ **Paper** – Open hand (all fingers up)
   - ✌️ **Scissors** – Index and middle fingers up
4. The AI will make its move, and the game will display both moves along with the updated scores.
5. Press **`s`** again to play another round!

## 🧠 How It Works

1. **Hand Detection** – MediaPipe detects 21 landmarks on your hand and draws them on screen in real time.
2. **Finger Counting** – The program checks the position of each fingertip relative to its base joint to determine if the finger is open or closed.
3. **Gesture Classification**:
   - All fingers closed → **Rock**
   - All fingers open → **Paper**
   - Index and middle finger open, others closed → **Scissors**
4. **Game Logic** – Compares the player's gesture with a randomly generated AI move, determines the winner, and updates the scoreboard.

## 📁 Project Structure
ROCK-paper-Scissor/
│
├── Resources/           # Images/assets used in the game (icons, backgrounds, etc.)
├── main.py              # Main game logic — hand detection, gesture classification, game loop
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
## 🔮 Future Improvements

- Add sound effects for countdown and results
- Support multiplayer mode (two-hand detection)
- Display gesture confidence percentage
- Web deployment using Flask/Streamlit
- Best-of-N rounds tournament mode

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## 📄 License

This project is licensed under the Apache License 2.0

## 👤 Author

**Your Name**
- GitHub: [@Bhuvan07-11](https://github.com/Bhuvan07-11))
