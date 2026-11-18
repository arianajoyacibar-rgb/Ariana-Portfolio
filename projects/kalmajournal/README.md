# Kalma

A private mood journal for students. Check in with how you feel, add a few lines, and see your mood over time. When a rough patch lasts, Kalma gently suggests talking to someone and shows how to reach help.

## Features
- Five-point mood check-in, topic tags and an optional journal entry
- On-device sentiment analysis using a small English and Filipino word list, shown as a "tone" label
- 14-day mood chart with a 3-day average, streak and averages
- **Gentle outreach**: three low days in a row shows a supportive prompt; language of self-harm shows the NCMH Crisis Hotline (1553) and 911 immediately
- **Talk to someone**: leave a message for the guidance office, anonymous or named (prototype: saved locally)
- **Counselor view**: anonymous group-level numbers only, with small groups hidden (sample data)
- Privacy by design: all data stays in the browser; export or delete any time

## Run
Open `index.html`. Use **Privacy → Load 14 days of sample data** to see the chart and the rough-week prompt.

## Ethics notes
- The tone label and prompts are suggestions, not diagnoses, and are never shown to anyone else
- A school deployment needs student consent, a Data Privacy Act review and a clear plan for who responds, built with the guidance office
- The word-list approach is simple and can be wrong (sarcasm, slang). A thesis version should evaluate it against labeled data and with counselor input

## Thesis angles
- Compare a word-list baseline with a trained classifier on Filipino and Taglish text
- Pilot with a small group and measure usability and willingness to reach out
