# Navaneeth KG

I build things where hardware, software and manufacturing meet: embedded
firmware, mecanum robots on ROS 2, computer-vision prototypes, and tooling for
running a small fleet of 3D printers.

## What I work on

| Area | What that means in practice |
|---|---|
| Embedded | ESP32, ATmega328P / ATmega32A, STM32; I2C / SPI / UART peripherals (INA219, MPU6050, NRF24L01, SSD1306, ST7735); motor drivers, encoders, battery and solar power |
| Robotics | ROS 2 Humble on Raspberry Pi, mecanum drive, LiDAR and depth cameras, odometry and SLAM |
| Computer vision / applied AI | PyTorch, OpenCV, YOLO, NCNN and edge inference; FastAPI and PyQt front ends |
| 3D printing | Bambu Lab P1S / A1 / A1 Mini with AMS, batch production, G-code, costing and capacity planning |
| Software | Python, C/C++, JavaScript / TypeScript, Flutter; Discord bots and automation |

## Projects

| Project | What it is | Stack |
|---|---|---|
| [lidar-slam-lab](https://github.com/projectbin07-stack/lidar-slam-lab) ([live demo](https://projectbin07-stack.github.io/lidar-slam-lab/)) | Browser sandbox for 2D LiDAR: occupancy-grid mapping, scan matching and particle-filter localisation, with live error metrics | JavaScript, no dependencies |
| [pid-tuning-lab](https://github.com/projectbin07-stack/pid-tuning-lab) ([live demo](https://projectbin07-stack.github.io/pid-tuning-lab/)) | Browser lab for tuning discrete PID controllers on motor, thermal and other plant models: anti-windup, autotuning, Bode / Nyquist and stability margins | JavaScript, no dependencies |
| [printfarm-planner](https://github.com/projectbin07-stack/printfarm-planner) | Schedules print jobs across a mixed Bambu fleet with AMS, nozzle, bed and staffed-hours constraints; HTML Gantt report | Python (stdlib) |
| [stl-doctor](https://github.com/projectbin07-stack/stl-doctor) | Checks STL / 3MF meshes before slicing: holes, flipped faces, overhangs, thin walls, bed fit; opt-in repair and an HTML report with drawn views | Python (stdlib) |
| [dataset-audit](https://github.com/projectbin07-stack/dataset-audit) | Audits image datasets (folder, YOLO, COCO) before training: corrupt files, near-duplicates, train/test leakage, label errors, class balance; CI exit codes | Python, NumPy, Pillow |
| [gcode-insight](https://github.com/projectbin07-stack/gcode-insight) | Analyse FDM G-code without a printer: layers, filament, time estimate, cost and price per print or batch, HTML report | Python |
| [mecanum-kinematics](https://github.com/projectbin07-stack/mecanum-kinematics) | Inverse / forward kinematics, SE(2) odometry and a deterministic simulator for 4-wheel mecanum robots, usable with or without ROS 2 | Python, NumPy |
| [rosbag-inspect](https://github.com/projectbin07-stack/rosbag-inspect) | Health-checks ROS 2 bags (SQLite3 and MCAP) without a ROS install: rates, gaps, latency, TF tree, LiDAR / IMU / odometry sanity; HTML report and CI exit codes | Python (stdlib) |
| [encoder-odometry-firmware](https://github.com/projectbin07-stack/encoder-odometry-firmware) | Four-wheel quadrature decoding, per-wheel velocity control and odometry for ESP32 / STM32, with a COBS + CRC serial protocol and a Python host bridge | C++, PlatformIO, Python |
| [serial-scope](https://github.com/projectbin07-stack/serial-scope) | Serial monitor, logger and live plotter for Windows and Linux that decodes structured telemetry (Arduino plotter, CSV, JSON, CRC-checked binary frames) and replays logs exactly | Python, tkinter |
| [ina219-battery-monitor](https://github.com/projectbin07-stack/ina219-battery-monitor) | INA219 battery and power telemetry firmware with OLED display, coulomb counting and a host logger | C++, PlatformIO |
| [tickreplay](https://github.com/projectbin07-stack/tickreplay) | Deterministic event-driven backtesting and paper-trading research engine with no look-ahead | Python (stdlib) |
| [xray-analysis-aiml](https://github.com/projectbin07-stack/xray-analysis-aiml) | Dashboard around the pretrained TorchXRayVision chest X-ray classifier, with optional local-LLM explanation | PyTorch, FastAPI |
| [wound-analysis-aiml](https://github.com/projectbin07-stack/wound-analysis-aiml) | U-Net wound segmentation with image-derived metrics and a dashboard | PyTorch, FastAPI, OpenCV |

Every repository has tests and CI, and each README says what has and has not
been verified. The firmware and robotics projects are tested in simulation and
on the host; where something has not yet run on real hardware, it says so. The
two medical-imaging projects are research prototypes, not medical devices. The
backtester ships only synthetic data and makes no performance claims.

I also build the software behind BRYKLE, a 3D-printing business; that code is
private.

## Contact

[LinkedIn](https://www.linkedin.com/in/navaneeth-2a5298369/)
