# Face-Recognition

> A webcam photo-capture and email demo — it does not perform face recognition.

## Overview

The browser asks for camera permission, captures an image, and sends it to a small Flask endpoint that emails the image. The repository name overstates the current implementation; no face-matching or identity-recognition feature is present in the checked code.

## What’s in this repo

- Browser camera preview and user-initiated capture
- Flask endpoint for receiving and emailing the captured image
- A small proof of concept for browser media APIs and image handling

## Stack

Python, Flask, browser JavaScript, SMTP.

## Getting started

1. Install Python and Flask, then configure mail settings for a test account.
2. Run `python app.py` and open the local page in a browser that supports camera access.
3. Grant camera permission only when you intend to capture an image.

## Notes

The checked source contains placeholder mail values. Do not put real credentials in source code; use a safer secret configuration before adapting this demo. Send images only with the subject's informed consent.
