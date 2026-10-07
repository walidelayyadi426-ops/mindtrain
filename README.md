# Memory Training 🧠

A production-ready offline cognitive exercise collection built with Flutter. Designed specifically for reliable Google Play Console testing, zero permissions, and 100% compliance with Google Play Store policies.

---

## 🎯 Google Play Console Warm-up & Safety Compliance

| Google Play Policy Area | Configuration & Guarantee |
| :--- | :--- |
| **Runtime Permissions** | **0 Permissions**. No camera, storage, microphone, location, contacts, or Bluetooth. |
| **Network & Internet** | **100% Offline**. Zero external API calls. Release manifest contains **no** `INTERNET` permission. |
| **Data Safety Form** | Answer **"No"** to all data collection and sharing questions. |
| **Ads Declaration** | Select **"No, my app does not contain ads"**. |
| **Target Audience** | Choose **18 and older** (avoids strict Designed for Families / COPPA policies). |
| **User Accounts** | **No accounts / login**. 100% immune to Google’s Account Deletion mandate. |
| **Medical Policy** | Strictly casual entertainment & memory training. Zero medical or health claims. |

---

## 🎮 Playable Games Included

1. **Memory Match**
   - 3 difficulty modes: Easy (4x4), Medium (4x6), Hard (6x6).
   - Card flip feedback, match validation, move counter, and timer.
2. **Sequence Memory**
   - 3x3 interactive pad with animated step replay (Simon-style).
   - Progressive difficulty with sequence length, 3 lives, and longest sequence tracking.
3. **Number Memory**
   - Digits displayed with animated countdown progress bar.
   - Built-in numeric keypad with backspace and confirmation.
   - Digits increase on success; 3 lives.
4. **Pattern Memory**
   - 4x4 matrix where target cells highlight briefly.
   - User taps the remembered positions; level increases progressively.
5. **Quick Recall**
   - 3 multi-item memory rounds.
   - Distractors and choices with real precision calculation (correct picks, false positives).

---

## 📅 Daily Challenge Mode

- Deterministic daily seed generated from the local calendar date (`DateTime.now().year * 10000 + month * 100 + day`).
- Consistent 3-game challenge across players on any given calendar day without requiring an internet connection.
- Distinguishes official 1st attempt from practice runs.

---

## 📈 Progression & Local Storage

- **Level System**: 6 progression tiers (Beginner, Learner, Focused, Advanced, Expert, Master) driven by actual earned XP.
- **Streak System**: Calendar-based streak incrementing when played consecutively, resetting if a day is missed.
- **Personal Records**: Best times, longest sequences, max digits, best pattern levels.
- **Recent Sessions**: Visual chart of accuracy and score across the last 7 sessions.
- **Storage**: Lightweight, persistent offline storage via `shared_preferences`.

---

## 🛠️ Testing & Verification

Run tests:
```bash
flutter test
```

Run static analysis:
```bash
flutter analyze
```

# mindtrain
