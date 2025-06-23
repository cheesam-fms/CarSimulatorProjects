# 🕹️ Logitech Wheel Controller – Driving Force GT

## 🎮 Device Overview
The **Driving Force GT** is an older Logitech racing wheel, originally designed for PlayStation and PC. While it still functions well for basic input, it has limited compatibility with modern Logitech SDKs and force feedback systems in Unity.

---

## 🔗 SDK & Driver Support

- 🔧 **Logitech Gaming Software (LGS)**  
  [Download for DFGT](https://support.logi.com/hc/en-my/articles/360024699474--Downloads-Driving-Force-GT)

- 🧰 **Unity Logitech SDK**  
  [Unity Asset Store – Logitech Gaming SDK](https://assetstore.unity.com/packages/tools/integration/logitech-gaming-sdk-6630#reviews)

- ⚠️ **Not Compatible with G HUB**  
  DFGT uses **Logitech Gaming Software (LGS)**, whereas newer wheels like **G29** and **G923** require **G HUB**.  
  The links below are intended **only for newer devices**:

  - 🛠️ [LogitechSteeringWheel.dll Fix (YouTube)](https://www.youtube.com/watch?v=2PGa0DV_a08)
  - 🔬 [Official Logitech Developer Lab SDKs](https://www.logitechg.com/en-gb/innovation/developer-lab.html)

---

## 🎥 Testing & Gameplay Demos

- 📹 [DFGT Unity Testing (uses `"Horizontal"` input)](https://www.youtube.com/watch?v=1mqwgfovrWY)  
- 📹 [DFGT Review with Gameplay Compatibility (starts at 15:49)](https://www.youtube.com/watch?v=CMY5Uq7tS-A)

---

## 💬 Community Discussions

- 🧵 [Unity DLLNotFoundException – `LogitechSteeringWheel`](https://discussions.unity.com/t/dllnotfoundexception-logitechsteeringwheel-unity5-osx/580619/5)  
- 🧵 [StackOverflow – Unity Logitech SDK can't detect G29](https://stackoverflow.com/questions/51001470/unity-logitechsdk-cannot-detect-my-g29-steering-wheel)

---

## 🧪 Test Notes

- ✅ **Input Detection**:  
  The Logitech Gaming Software successfully detects the DFGT and allows **basic input mapping** (e.g., `Input.GetAxis("Horizontal")` in Unity).

- ❌ **SDK Incompatibility**:  
  The Unity Logitech SDK (`LogitechSteeringWheelEngine.dll`) is **not compatible** with the version of Logitech Gaming Software used for the DFGT. Force feedback and advanced features do not function via the SDK.

- ⚙️ **Alternative for Force Feedback**:  
  Try using **[Unity-DirectInput](https://github.com/imDanoush/Unity-DirectInput)** as an alternative method to access **Force Feedback** via raw DirectInput.

---

> ✅ The DFGT works with Unity’s built-in input system for simple driving games.  
> ❗ Use caution when expecting SDK-based advanced features like force feedback, as they may not be supported with this older wheel.
