# Audio Transcription & Diarization SOP

Standardized formatting guidelines for speech-to-text (ASR) training data, speaker diarization, and acoustic event tagging.

## 1. Speaker Labeling Convention
* **`[SPEAKER_01]`**, **`[SPEAKER_02]`**: Assign sequential IDs based on first appearance.
* **`[OVERLAP]`**: Used when two or more speakers talk simultaneously and intelligibility is affected.

## 2. Non-Speech & Acoustic Event Tags
* **`[NOISE]`**: Background environmental interference (traffic, wind, mic handling).
* **`[LAUGHTER]`** / **`[COUGH]`**: Paralinguistic vocalizations produced by the active speaker.
* **`[UNINTELLIGIBLE]`**: Speech masked by heavy distortion or low signal-to-noise ratio.

## 3. Verbatim vs. Clean-Read Rules
* **Verbatim Mode (ASR Training):** Retain filler words (`उम`, `मतलब`, `uh`, `like`), false starts, and regional code-switching without grammatical correction.
* **Code-Switching Standard:** Transcribe Hindi words in Devanagari script and embedded English terms in Latin script (e.g., `"आज की meeting में dataset पर चर्चा हुई।"`).
