# Whatsapp-Chat-Analyser-Project
This repository is a Whatsapp Chat Analyser which is a Data Science Project.

# GroupDNA - WhatsApp Group Chat Analyzer

**Spotify Wrapped, but for your friend group.**

A Python-based analytics tool that analyzes WhatsApp group chat exports to generate comprehensive personality and activity reports.

## 📊 Project Overview

GroupDNA analyzes raw WhatsApp chat export files to identify patterns in messaging behavior, assign personality archetypes to participants, and visualize group dynamics through text-based analytics.

### Dataset Information
- **File:** `hostel_bois.txt` (synthetic WhatsApp chat export)
- **Participants:** 6 (Rahul, Priya, Aman, Karan, Neha, Vikas)
- **Date Range:** 01 April 2024 to 30 May 2024 (60 days)
- **Total Messages:** 3,174

## 🚀 Features

### 1. Chat Parser
- Reads WhatsApp chat export files line by line
- Extracts timestamp, sender, and message text
- Handles edge cases: system messages, media-omitted, deleted messages

### 2. Group Overview
- Total messages and date range
- Participant count
- Per-person message distribution with percentages

### 3. Word Frequency Analysis
- Extracts and counts words from all messages
- Identifies top 10 most-used words
- Visual bar representation of word frequency

### 4. NumPy Activity Heatmap
- Text-based heatmap showing message activity by hour
- Uses NumPy for matrix operations
- Visual representation with block characters (░, ▒, █)

### 5. Response Times & Silent Streaks
- Average response time per participant
- Longest silent streak (consecutive days with zero messages)
- Identifies fastest and slowest repliers

### 5.5. Most Active Day and Hour
- Identifies the most active day in the chat period
- Identifies the most active hour (24-hour format)
- Displays top 5 most active days
- Shows hourly message distribution with visual bars

### 6. Personality Archetype Detection
Assigns one of 8 archetypes to each participant:
- **THE SPAMMER** - High consecutive message bursts
- **THE GROUP MOM** - Caring keywords usage
- **THE NIGHT OWL** - Late-night messaging pattern
- **THE STORYTELLER** - Long messages
- **THE DRAMA QUEEN** - ALL-CAPS or multiple exclamations
- **THE GHOST** - Silent majority of days
- **THE COMEDIAN** - Laughter words usage
- **THE QUESTION MASTER** - High question frequency

### 7. Final Report
- Comprehensive, beautifully formatted output
- Visual hierarchy with box-drawing characters
- Screenshot-ready terminal aesthetics

## 🛠️ Technology Stack

- **Python 3.x** - Core language
- **NumPy** - Matrix operations for heatmap
- **datetime** - Time parsing and calculations
- **Built-in libraries only** - No pandas, matplotlib, or external packages

## 📋 Constraints Followed

✅ No pandas used for file reading (used Python's built-in `open()`)  
✅ No matplotlib used for heatmap (used text-based rendering with NumPy)  
✅ No collections.Counter used (built custom word counter with dict)  
✅ Only Python fundamentals + NumPy + datetime used  
✅ All 8 features implemented  
✅ Proper file I/O with UTF-8 encoding  
✅ Clean, formatted output with visual hierarchy  
✅ Proper error handling for edge cases  

## 🏃 How to Run

### Local Execution
1. Ensure Python 3.x is installed
2. Install NumPy: `pip install numpy`
3. Place `hostel_bois.txt` in the same directory as the notebook
4. Open `GroupDNA_Student_DS24007.ipynb` in Jupyter Notebook
5. Run all cells from top to bottom

### Google Colab
1. Upload `GroupDNA_Student_DS24007.ipynb` to Google Colab
2. Upload `hostel_bois.txt` to the Colab session files
3. Run all cells sequentially

## 📁 Project Structure

```
.
├── GroupDNA_Student_DS24007.ipynb  # Main notebook
├── hostel_bois.txt                  # Dataset file
├── README.md                        # This file
└── GroupDNA_Minor_Project_Brief.pdf # Project requirements
```

## 🎯 Learning Outcomes

- File I/O operations with UTF-8 encoding
- String parsing and text processing
- Data structure manipulation (lists, dictionaries, sets)
- NumPy matrix operations
- Datetime parsing and time calculations
- Pattern detection and rule-based classification
- Output formatting and visual design

## 📝 Notes

- The dataset is synthetic and designed for this project
- Each participant has deliberately engineered personality patterns
- The notebook can be adapted to analyze real WhatsApp exports
- Multi-line message handling is not implemented (dataset doesn't require it)

## 🎓 Academic Context

This is a Week 1 industry-graded minor project for The Unlox Academy Data Science program. The project emphasizes:
- Constraint discipline (no shortcuts with pandas/matplotlib)
- Fundamentals-first approach
- Real-world data cleaning experience
- Shareable, visual output design

## 📸 Sample Output

The final report generates a terminal-formatted analytics report with:
- Box-drawing characters for visual hierarchy
- Aligned columns with proper spacing
- Block character bars for visual data representation
- Clear section dividers and headers

---

**Generated by GroupDNA Analyzer | Python Fundamentals + NumPy**

