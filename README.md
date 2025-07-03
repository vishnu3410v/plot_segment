#  ECG Segment Visualizer

This simple yet powerful script allows you to visualize a **specific time segment** of an ECG waveform from a `.csv` file converted from the MIT-BIH Arrhythmia Database.

The user simply enters the **start and end time (in seconds)**, and the script will extract and plot that portion of the ECG signal.

---

##  What It Does

-  Loads ECG data from a `.csv` file (e.g., generated using WFDB)
-  Takes user input for a **start** and **end** time (in seconds)
-  Extracts only that portion of the signal
-  Plots the extracted signal for visual inspection

---

##  Project Structure

   
    ecg_segment_viewer/
    ├── csv_output/ # Folder containing .csv ECG data
    ├── plot_segment.py # This script
    └── README.md # You're reading it!


---

##  Requirements

- `pandas`
- `matplotlib`

Install using:

```
pip install pandas matplotlib

```
 How to Run

1. Save the Script
Save the following as `plot_segment.py`

2.  Provide Input When Prompted
Run the script:
 ```  
python plot_segment.py
```
Then input the start and end times when prompted (e.g., 5 and 10 to see seconds 5–10 of the waveform).

🧪 Example
If your ECG CSV has a MLII column and you enter:
```
Enter start time in seconds: 5
Enter end time in seconds: 10
```
You’ll see a plot of that 5-second ECG segment.

🧠 Tips
- Make sure your CSV has a proper signal column name (MLII, V1, etc.)

- This tool is especially useful for zooming into arrhythmia windows or peak intervals

- Can be easily extended to highlight R-peaks or QRS complexes

📜 License
MIT — free to use and modify.





