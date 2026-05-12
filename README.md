# ConCrete-Capillary-Absorption-Timer 🔬

**A real-time Laboratory Execution System  for precision sorptivity testing in material science.**

---

## 📖 Overview

In durability studies of cementitious binders, managing the weighing schedule for dozens of specimens is a logistical challenge. Capillary absorption (sorptivity) is measured at square-root-of-time intervals ($t^{0.5}$); even a 60-second deviation can introduce "jitter" into the curve, compromising the accuracy of the sorptivity coefficient.

This browser-based tool was developed during my Ph.D. research at the **University of Navarra** to eliminate human error and provide a "gloves-ready" interface for high-volume specimen testing.

---

## 🚀 Key Features

*   **Dynamic Task Injection:** Enter the initial "Dry Mass" ($M_0$) for a specimen, and the system instantly calculates and schedules all future intervals based on standard protocols (e.g., ASTM C1585).
*   **Real-Time "Urgent" Alerts:** Rows dynamically change color (Red/Yellow) the moment a sample is due, ensuring zero missed measurements.
*   **Input Stability Lock:** Custom logic prevents table refreshes or "jumps" while data is being entered—critical for fast-paced lab environments.
*   **Precision Logging:** Records the *actual* timestamp of every entry (not just the scheduled time) to allow for perfect data correction during post-processing.
*   **Zero-Install Portability:** A single lightweight HTML/JS file that runs in any browser. No database, server, or installation required.

---

## 🛠️ How to Use

1.  **Setup:** Define your experiment name, number of groups, and specimens.
2.  **Initialize:** Enter specimen dimensions ($D_1, D_2$) to establish the absorption surface area.
3.  **Start:** As you weigh and place each dry sample into the water, hit "Enter." The system maps that specific sample's unique timeline.
4.  **Export:** Click **"EXPORT PRECISION DATA"** to download a `.csv` file formatted for immediate plotting in Excel, Origin, or Python.

---

## 📊 Data Export Format

The system generates an analysis-ready `.csv` file containing:
*   **Specimen ID & Group**
*   **Target Interval:** The theoretical $t^{0.5}$ mark.
*   **Actual Timestamp:** The exact second the data was logged.
*   **Mass Measurement:** The recorded weight at that interval.
*   **Surface Area:** Automatically calculated from input dimensions.

---

## 🤖 AI Collaboration

This tool serves as a case study in **Human-AI collaboration**. By combining domain expertise in **Material Chemistry** with generative AI, the transition from conceptual logic to a functional laboratory tool was achieved in a fraction of the time required for traditional software development.


---

## ✍️ Author
**Mohammad Hossein Nofalah**  
*Ph.D. Candidate & Researcher*  
**University of Navarra** | Materials and Cultural Heritage (MATCH) Group

---

> **Note:** To use this tool, simply download the `index.html` file and open it in any modern browser (Chrome, Firefox, or Edge). No internet connection is required once the file is saved locally.
