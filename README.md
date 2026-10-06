# Webcam-To-Email

A small Flask utility: capture a photo from the browser webcam and email it to a configured address.

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Web%20Framework-green)](https://flask.palletsprojects.com/)
[![License](https://img.shields.io/badge/License-MIT-yellowgreen)](LICENSE)
[![Commits](https://img.shields.io/github/commit-activity/m/neerajsait/Face-Recognition)](https://github.com/neerajsait/Face-Recognition/commits/main)

## About this project

This repository is part of **Neeraj Sai's** growing collection of software projects, experiments, and learning builds. It reflects a practical, curious approach to creating useful products and understanding how they work under the hood.

This is a utility experiment, not a face-recognition system. It performs no biometric identification. I built this to explore how browser webcam access works and how to handle image data on the backend securely.

## How it works

1. The page requests webcam access via `getUserMedia`.
2. A captured frame is sent to the Flask backend as base64.
3. The backend emails the image via SMTP.

## Tech Stack

- **Backend** — Python 3.8+, Flask, SMTP
- **Frontend** — HTML, JavaScript

## Installation & Setup

### Prerequisites
- Python 3.8+
- A Gmail account (enable 2FA and create an [App Password](https://support.google.com/accounts/answer/185833))

### Steps

1. **Clone the repo**
   ```bash
   git clone https://github.com/neerajsait/Face-Recognition.git
   cd Face-Recognition
   ```

2. **(Recommended) Create a virtual environment**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Linux/macOS:
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install flask python-dotenv
   ```

4. **Configure email**
   Set `EMAIL_ADDRESS`, `EMAIL_PASSWORD` (app password), and `RECIPIENT_EMAIL` in `app.py` (or use `.env`), then run `python app.py`.

5. **Run the app**
   ```bash
   python app.py
   ```

6. **Open in browser**
   Visit `http://localhost:5000` to test the capture and email flow.

## Note

This is a utility experiment, not a face-recognition system. It performs no biometric identification.

## Author

**Tiruveedhi Neeraj Venkata Sai**
- GitHub: [@neerajsait](https://github.com/neerajsait)
- Portfolio: [neeraj's portfolio](https://github.com/neerajsait/portfoliomain)

## License

MIT License — see the LICENSE file for details. Built in my free time by @neerajsait.
