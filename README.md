# Assembly: Endgame

A programming-themed hangman game built with React where you must guess words to save the programming world from Assembly language!

## 🎮 Game Overview

Assembly: Endgame puts a fun twist on the classic hangman game. Instead of drawing a hangman, each wrong guess eliminates a programming language from existence. Your mission is to guess the word within 8 attempts to keep all programming languages safe from the dreaded Assembly takeover!

## ✨ Features

- **Programming Theme**: Features 9 popular programming languages as "lives"
- **Interactive Keyboard**: Click letters to make guesses
- **Visual Feedback**: 
  - Correct letters turn green
  - Wrong letters turn red
  - Lost languages show a skull overlay
- **Accessibility**: Screen reader support with ARIA labels and live regions
- **Responsive Design**: Works on desktop and mobile devices
- **Random Words**: Large dictionary of English words for variety

## 🚀 Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd assembly-endgame
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and navigate to `http://localhost:5173`

## 🎯 How to Play

1. **Objective**: Guess the hidden word by selecting letters
2. **Lives**: You have 8 attempts (represented by programming languages)
3. **Making Guesses**: Click on letters in the on-screen keyboard
4. **Winning**: Reveal all letters in the word before running out of attempts
5. **Losing**: Make 8 incorrect guesses and Assembly takes over!

### Programming Languages (Your Lives)
- HTML
- CSS  
- JavaScript
- React
- TypeScript
- Node.js
- Python
- Ruby
- Assembly (the final boss!)

## 🛠️ Technical Details

### Built With
- **React 18** - UI framework
- **Vite** - Build tool and dev server
- **CSS3** - Styling with custom properties
- **clsx** - Conditional CSS classes

### Project Structure
```
src/
├── App.jsx          # Main game component
├── languages.js     # Programming language data
├── words.js         # Word dictionary
├── utils.js         # Helper functions
├── index.css        # Global styles
└── main.jsx         # App entry point
```

### Key Components

#### Game State Management
- Uses React hooks (`useState`) for state management
- Tracks current word, guessed letters, and game status
- Derived state for win/loss conditions

#### Accessibility Features
- ARIA labels for screen readers
- Live regions for dynamic content updates
- Keyboard navigation support
- High contrast colors for visibility

#### Visual Design
- Dark theme with vibrant accent colors
- Each programming language has its authentic brand colors
- Smooth transitions and hover effects
- Mobile-responsive layout

## 🎨 Customization

### Adding New Words
Edit `src/words.js` to add or modify the word list:

```javascript
export const words = [
  "your-new-word",
  // ... existing words
];
```

### Modifying Languages
Update `src/languages.js` to change programming languages:

```javascript
export const languages = [
  {
    name: "Your Language",
    backgroundColor: "#COLOR",
    color: "#TEXT_COLOR",
  },
  // ... other languages
];
```

### Styling Changes
- Global styles: `src/index.css`
- Component-specific styles: Embedded in CSS classes

## 🧪 Game Logic

### Win Condition
Player wins when all letters in the current word have been guessed correctly.

### Loss Condition  
Player loses when they make 8 incorrect guesses (one for each programming language except Assembly).

### Farewell Messages
When a programming language is eliminated, a random farewell message is displayed, adding personality to the game.

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Preview Production Build
```bash
npm run preview
```

The built files will be in the `dist/` directory, ready for deployment to any static hosting service.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

---

**Save the programming world from Assembly! Start playing now! 🚀**
