# 🎤 Speaker Recognition for User Authentication (MATLAB DSP)

## Project Poster 
<img width="1002" height="755" alt="image" src="https://github.com/user-attachments/assets/46b7add7-d921-418a-9260-b96acf83c6d9" />


---

## 📌 Overview

This project implements a **text-dependent speaker verification system** using Digital Signal Processing techniques in MATLAB.
It authenticates a user by comparing an **authorized voice sample** with a **test voice sample**.

---

## 🚀 Key Features

* Speaker authentication using voice signals
* Noise reduction with bandpass filtering
* Feature extraction using **MFCC**
* Pattern matching using **DTW (Dynamic Time Warping)**
* Automatic signal visualization (time & frequency domain)

---

## 📂 Project Structure

```text
Speaker-Recognition-MATLAB/
│── main.m
│── README.md
│── assets/
│     └── poster.png
│── sample_audio/   (optional)
│── OUTPUT_PLOTS/   (generated automatically)
```

---

## ⚙️ Requirements

* MATLAB (R2020 or later recommended)
* Signal Processing Toolbox

---

## ▶️ How to Run

1. Open MATLAB
2. Navigate to project folder
3. Run:

```matlab
main
```

4. Select:

   * Authorized voice (.wav)
   * Test voice (.wav)

---

## 🧠 Working Pipeline

1. **Resampling** → Standardize to 48 kHz
2. **Bandpass Filtering** → 300 Hz – 3000 Hz
3. **Voice Activity Detection (VAD)** → Remove silence
4. **MFCC Extraction** → Feature extraction
5. **DTW Matching** → Compare voice patterns
6. **Decision** → Authenticate user

---

## 📊 Output

The system displays:

* DTW Distance
* Distance Ratio

Final result:

```
Same Speaker : Login Successful
OR
Different Speaker : Login Failed
```

---

## 📈 Generated Outputs

Saved in `OUTPUT_PLOTS/`:

* Time-domain signals
* Frequency-domain (FFT)
* Filter response

---

## ⚠️ Notes

* Input must be `.wav` files
* Works best with clean audio
* Designed for same-phrase (text-dependent) verification

---

## 💡 Future Improvements

* GUI-based interface
* Deep learning integration (CNN/RNN)
* Noise-robust feature extraction
* Real-time authentication system

---

