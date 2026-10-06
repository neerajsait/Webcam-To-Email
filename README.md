# Webcam-To-Email

A small Flask utility: capture a photo from the browser webcam and email it to a configured address.

## How it works
1. The page requests webcam access via `getUserMedia`.
2. A captured frame is sent to the Flask backend as base64.
3. The backend emails the image via SMTP.

## Tech
Python, Flask, JavaScript, HTML.

## Setup
Set `EMAIL_ADDRESS`, `EMAIL_PASSWORD` (app password), and `RECIPIENT_EMAIL` in `app.py`, then run `python app.py`.

## Note
This is a utility experiment, not a face-recognition system. It performs no biometric identification.
