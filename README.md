# AC Milan Game Reminder

This Python project is designed to send automated email reminders about AC Milan's game schedule. The script checks for upcoming games and sends a reminder to the specified email address at 7:00 AM MST on game days.

---

## Features

- Fetches AC Milan's game schedule (manually input or from an API).
- Sends automated email reminders to a specified email address.
- Scheduled to run daily at a fixed time (7:00 AM MST).
- Notifies about the competition, opponent, and game time.

---

## Requirements

- Python 3.7+
- Libraries:
  - `schedule`: For task scheduling.
  - `smtplib`: For sending emails via SMTP.
  - `pytz`: For handling timezone conversions.
  - `email`: For formatting email content.

Install required libraries using:
```bash
pip install schedule pytz
```

---

## Setup and Configuration

1. Clone the repository:
   ```bash
   git clone https://github.com/sosika/acmilan_reminder.git
   cd acmilan_reminder
   ```

2. Add your email credentials in the script:
   - Replace `your_email@gmail.com` with your sender email.
   - Replace `your_email_password` with your email's app password (for Gmail, generate an [App Password](https://support.google.com/accounts/answer/185833?hl=en)).

3. Update the game schedule:
   - Edit the `get_ac_milan_schedule()` function to include the latest AC Milan schedule.
   - Optionally, integrate with a football API for dynamic schedule fetching.

4. Run the script:
   ```bash
   python game_reminder.py
   ```
   Keep the script running to ensure daily reminders are sent.

---

## How It Works

1. The script checks the AC Milan schedule to identify if there is a game on the current date.
2. If a game is found, it sends an email reminder at 7:00 AM MST.
3. The email includes:
   - Opponent name
   - Competition (e.g., Serie A, Coppa Italia)
   - Game time

---

## Example Email

**Subject:** AC Milan Game Reminder  
**Body:**
```
Today's games:

AC Milan vs Inter Milan
Competition: Serie A
Time: 20:45 MST
```

---

## Enhancements

Future improvements to the project could include:

1. Fetching schedules dynamically from a sports API.
2. Adding desktop notifications in addition to email reminders.
3. Expanding to include live game scores or updates.
4. Supporting multiple recipients or group reminders.

---

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute as needed.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your proposed changes.



