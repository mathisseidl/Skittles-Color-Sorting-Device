🎨 Skittles Color Sorting Device

__📌 Overview__

This project is a **low-cost, portable, and accessible** candy color sorting device designed to automatically sort Skittles into five colors: **Red, Yellow, Green, Orange, and Purple.**
A key design goal was accessibility, the device can be used by **color-blind and visually impaired users**, featuring engraved labels and **Braille markings** for each output compartment.

__🚀 Key Features:__

✅ Sorts 5 colors (Red, Yellow, Green, Orange, Purple)

🎯 99% accuracy across 100 trials

⏱ Fast operation (~3 seconds per Skittle)

♿ Accessible design (Braille + engraved labels)

🔋 Fully portable (battery-powered)

🧩 Modular & serviceable (17 custom 3D-printed parts)

__🛠️ System Architecture__
* Arduino Uno – main controller

TCS3200 RGB Color Sensor – color detection

MG996R Servo Motor – candy transport disc

S51 Micro Servo – ramp positioning

Vibration Motors – clog prevention

Power Supply

4× AA batteries (servos)

9V battery + buck converter (Arduino)

Mechanical Design

Wooden base for lightweight structure and laser engraving

Large funnel capacity (~50 Skittles)

Five individual storage compartments

17 custom 3D-printed parts (PLA)

🧠 How It Works

Candy is dropped into the funnel

A rotating disc moves the Skittle to the sensing position

The TCS3200 sensor takes multiple RGB readings

Color is classified using:

Normalized RGB ratios

Nearest-neighbor comparison

Two consecutive matching detections for noise filtering

A servo-controlled ramp guides the candy into the correct bin

System resets for the next cycle
