# 🚗 Vehicle Charging Reminder – Home Assistant Blueprint

Keep your EV or hybrid topped up without worrying about forgetting to plug it in! ⚡  

This **Home Assistant blueprint** sends a friendly mobile app notification if your vehicle is at home 🏠, the battery drops below your chosen threshold, and it isn’t plugged in. You can snooze the reminder ⏰ or ignore it completely ❌ — all from your phone!

---

## Features ✨

- ✅ Trigger reminders only when your vehicle is **home**  
- ✅ Works with **any battery sensor**  
- ✅ Stop reminders automatically if the car is **plugged in**  
- ✅ Mobile app notification includes **current battery %**  
- ✅ Actionable buttons:  
  - **Remind me later** - Snooze reminder for a set amount of minutes
  - **Ignore** - dismiss notifications
- ✅ Configurable **battery threshold**, **snooze time**, and **reminder time**  
- ✅ Perfect for **Home Assistant Companion App** on iOS & Android  

---

## Installation 🚀
[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fstumiles86%2FVehicleChargingReminder%2Fblob%2Fmain%2FVehicleChargingReminder.yaml)

or manually:

1. Download the blueprint YAML file from this repo  
2. Place it in your Home Assistant folder:
3. Go to **Settings → Automations & Scenes → Blueprints → Import Blueprint** in Home Assistant  
4. Select the blueprint and create your automation using your sensors and mobile device  

---

## Inputs 📝

- **Car Battery Sensor:** Your vehicle’s battery percentage sensor  
- **Vehicle Tracker:** Track when your car is at home  
- **Home Zone:** The zone where the reminder should trigger  
- **Charger Status Sensor:** Detect if the car is plugged in  
- **Charger Connected State:** The value that indicates “plugged in”  
- **Battery Threshold:** Battery % at which to notify you  
- **Reminder Time:** Daily time for the notification  
- **Notify Device:** Mobile app device that receives the reminder  
- **Reminder Text:** Optional custom message  
- **Snooze Minutes:** Time to wait before reminding again if snoozed  

---

## How it Works ⚡

1. At the configured **reminder time**, the blueprint checks:  
- Is the vehicle **home**? 🏠  
- Is the **battery below the threshold**? 🔋  
- Is the car **not plugged in**? 🔌  
2. If all conditions are met, a notification is sent to your mobile device.  
3. Notification includes **buttons**:  
- **Remind me later** → notification comes back after the snooze period  
- **Ignore** → stops further notifications for the day  

---

## Example Default Message 💬

> Vehicle battery is below 80% (currently at 65%). Please plug the vehicle in.

---

## Notes ⚠️

- Make sure you have the **Home Assistant Companion App** installed and notifications allowed.  
- Actionable buttons may require a **restart of the app** after importing the blueprint.  
- Works with **any EV, hybrid, or car battery sensor** compatible with Home Assistant.  

---

## Contribute / Feedback 🙌

Found a bug? Want to suggest features? Open an issue or submit a pull request.  

---

Keep your EV happy and avoid low-battery panic! 🔋🚗
