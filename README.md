# day-01-new-streak-2025-10-01
Start of my new GitHub streak. Daily commits with small scripts &amp; projects 🚀
#!/usr/bin/env python3
"""
Simple daily logger for the streak.
Usage:
    python app.py --note "what you did"
It appends a dated entry to log.json.
"""
import argparse, json, os
from datetime import datetime

LOG_FILE = "log.json"

def load_log():
    if not os.path.exists(LOG_FILE):
        return []
    with open(LOG_FILE, "r", encoding="utf-8") as f:
        try:
            return json.load(f)
        except Exception:
            return []

def save_log(data):
    with open(LOG_FILE, "w",_
