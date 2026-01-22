# Python Password Generator 🔐

A simple yet powerful password generator built with Python and Tkinter. This project creates secure, random passwords with customizable length and character repetition options.

## 📋 Features

- **Random Password Generation**: Creates strong passwords using a combination of:
  - Uppercase letters (A-Z)
  - Lowercase letters (a-z)
  - Numbers (0-9)
  - Special symbols (!#$%&'()*+,-./:;<=>?@[\]^_`{|}~)

- **Customizable Options**:
  - Set password length (recommended: 10+ characters)
  - Choose whether to allow character repetition

- **User-Friendly GUI**: Simple Tkinter interface for easy interaction

## 🚀 Getting Started

### Prerequisites

- Python 3.x installed on your system
- Tkinter (usually comes pre-installed with Python)

If Tkinter is not available (Linux systems), install it using:
```bash
sudo apt-get install python3-tkinter
```

### Installation

1. Clone this repository:
```bash
git clone <repository-url>
cd Python-Password--Generator-
```

2. Run the application:
```bash
python password_generator.py
```

## 💻 Usage

1. **Enter Password Length**: Input the desired length of your password (minimum 1 character)

2. **Choose Repetition Option**:
   - Enter `1` for no character repetition (each character appears only once)
   - Enter `2` (or any other number) to allow character repetition

3. **Generate Password**: Click the "Generate Password" button

4. **View Result**: Your generated password will appear in the read-only text field at the bottom

## 🔧 How It Works

### Key Components

1. **Imports**:
   - `random`: For generating random character selections
   - `tkinter`: For creating the GUI
   - `messagebox`: For displaying error prompts

2. **Character String**: Contains all possible characters for password generation

3. **Password Generator Function**:
   - Validates user inputs
   - Uses `random.sample()` for unique characters (no repetition)
   - Uses `random.choices()` for passwords with possible repetition
   - Displays the generated password in a read-only entry widget

4. **GUI Elements**:
   - Title label
   - Input fields for length and repetition preference
   - Generate button
   - Output display field

## 📝 Code Structure

```
password_generator.py
├── Imports (random, tkinter)
├── Character string definition
├── generate_password() function
├── GUI initialization
├── Input widgets (labels and entries)
├── Generate button
└── Main event loop
```

## 🎯 Example

- **Input**: Length = 16, Repetition = 1
- **Output**: `Created password: aB3!xZ9@mK7$pQ2&`

## 🛡️ Security Best Practices

- Use passwords with at least 10 characters
- Include a mix of uppercase, lowercase, numbers, and symbols
- Avoid using the same password across multiple platforms
- Store passwords securely using a password manager

## 🤝 Contributing

This is a beginner-friendly project. Feel free to fork and enhance it with additional features such as:
- Password strength indicator
- Copy to clipboard functionality
- Save passwords to file (encrypted)
- Multiple password generation at once

## 📄 License

This project is open source and available for educational purposes.

## 👨‍💻 Author

Created following the PythonGeeks tutorial - Perfect for Python beginners learning GUI development and the random module!

---

**Note**: This project is designed for educational purposes to help beginners understand Python GUI development with Tkinter and random string generation.
