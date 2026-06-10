# Student Council Election System 2026

A simple Flask-based digital voting system for conducting student elections securely within a school network.

## Features

* TS Number Login
* Valid TS Number Verification
* One Vote Per Student
* Head Boy Election
* Head Girl Election
* Automatic Vote Recording
* CSV-Based Storage
* Live Results API
* Admin Dashboard
* Responsive User Interface
* Local Network Support

---

## Project Structure

```text
project/

│ app.py
│ votes.csv
│ valid_ts_numbers.csv
│ requirements.txt
│ README.md

├── templates/
│   ├── login.html
│   ├── headboy.html
│   ├── headgirl.html
│   ├── thanks.html
│   └── admin.html

├── static/
│   ├── logo.png
│   ├── bg.jpg
│   ├── hb1.jpg
│   ├── hb2.jpg
│   ├── hb3.jpg
│   ├── hb4.jpg
│   ├── hg1.jpg
│   ├── hg2.jpg
│   ├── hg3.jpg
│   └── hg4.jpg
```

---

## Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Run Application

```bash
python app.py
```

Server starts on:

```text
http://127.0.0.1:5000
```

---

## Admin Dashboard

Open:

```text
http://127.0.0.1:5000/admin
```

Live API:

```text
http://127.0.0.1:5000/api/results
```

---

## CSV Format

### valid_ts_numbers.csv

```csv
TS001
TS002
TS003
TS004
```

### votes.csv

```csv
TIMESTAMP,TS_NO,HEAD_BOY,HEAD_GIRL
2026-06-09 10:30:22,TS001,Candidate 1,Candidate A
```

---

## Security Features

* Only approved TS Numbers can vote
* Duplicate voting prevention
* Session-based voting flow
* Votes stored locally
* No internet connection required

---

## Election Workflow

1. Student enters TS Number
2. TS Number is validated
3. Student votes for Head Boy
4. Student votes for Head Girl
5. Vote is recorded
6. Thank You page displayed
7. Student redirected to login page

---

## Developed For

Student Council Election 2026

The Study L'Ecole Internationale
