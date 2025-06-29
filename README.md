# 🎮 PlayStation 5 Controller Module

A lightweight and customizable module for interacting with the PlayStation 5 (DualSense) controller on desktop platforms. This project enables developers to integrate PS5 controller input features—like haptic feedback, triggers, gyroscope, and LED control—into their applications or games with ease.

---

## 📚 Table of Contents

- [Description](#description)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Known Bugs](#known-bugs)
- [Planned Features](#planned-features)
- [Contributors](#contributors)
- [Installation & Usage](#installation--usage)
- [Screenshots](#screenshots)
- [License](#license)

---

## 📝 Description

This module provides access to the PlayStation 5 DualSense controller inputs and outputs on PC, allowing for game development, testing, or personal automation. It supports real-time input reading, vibration control, LED color changes, and more.

It’s built to be cross-platform (Windows/macOS/Linux) and developer-friendly.

---

## 🚀 Features

- ✅ Detect DualSense connection/disconnection
- ✅ Read button presses, joystick, trigger input
- ✅ Access gyroscope and accelerometer data
- ✅ Control vibration (haptic feedback)
- ✅ Change LED light bar colors
- ✅ Trigger adaptive resistance settings

---

## 🛠 Technologies Used

- Python 3.10+ / Node.js (depending on your version)
- `pydualsense` or `hidapi` for low-level controller communication
- SDL2 or WebHID (optional)
- Git & GitHub
- VS Code / Terminal

---

## 🐞 Known Bugs

- 🐛 Vibration may not work on macOS (due to driver limitations)
- 🐛 Gyroscope sensitivity may vary across OS
- 🐛 Controller disconnecting during USB hot-plug on Linux

---

## 🧭 Planned Features

- [ ] Bluetooth support (currently only USB)
- [ ] Web dashboard to visualize controller data in real-time
- [ ] Game engine plugins (Unity/Unreal)
- [ ] Save/load custom LED profiles
- [ ] Controller battery level monitor

---

## 👥 Contributors

- Ashin Nafi ([@your-github-handle](https://github.com/your-github-handle)) – Creator & Lead Developer  
- Open to collaborators! Submit a PR if interested.

---

## 🧪 Installation & Usage

### Prerequisites

- A connected PlayStation 5 DualSense controller (USB)
- Python 3.10+ installed

### Installation (Python example)

```bash
git clone https://github.com/yourusername/ps5-controller-module.git
cd ps5-controller-module
pip install -r requirements.txt
python main.py
````

### Sample Code

```python
from ps5controller import DualSense

controller = DualSense()
controller.set_led_color("blue")
print("Press buttons on your DualSense...")

while True:
    controller.update()
    print(controller.button_state)
```

---

## 🖼 Screenshots

![Controller Input](images/controller-input-demo.png)
*Real-time input display*

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 🔗 Useful Links

* [Official DualSense Documentation](https://www.playstation.com/en-us/support/hardware/ps5-dualsense-wireless-controller/)
* [HIDAPI](https://github.com/libusb/hidapi)
* [pydualsense GitHub](https://github.com/flok/pydualsense)



