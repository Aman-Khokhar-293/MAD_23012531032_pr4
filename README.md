# ⏰ Android Alarm Application  

## 📌 AIM  
Create an Android Alarm application by using **Service** & **BroadcastReceiver**.  

---

## 📝 Explanation  
This application demonstrates how to schedule and handle alarms in Android using **AlarmManager**, **PendingIntent**, **BroadcastReceiver**, and **Service**.  

- **MainActivity** → User interface where the user selects the alarm time using **TimePickerDialog**.  
- **AlarmManager + PendingIntent** → Used to schedule the alarm at the selected time.  
- **BroadcastReceiver** → Triggered when the alarm time is reached, responsible for starting the **AlarmService**.  
- **AlarmService** → Plays the alarm sound using **MediaPlayer** and runs in the background.  
- **TextClock** → Displays current system time on the screen.  
- **MaterialCardView** → Provides a modern UI for Set/Cancel alarm buttons.  
- **Permissions** → The app requires `android.permission.SCHEDULE_EXACT_ALARM` in the manifest file to schedule exact alarms.  

**Flow of the Application:**  
1. User selects alarm time in **MainActivity**.  
2. **AlarmManager** sets the alarm with a **PendingIntent**.  
3. When the alarm triggers, **BroadcastReceiver** receives the intent.  
4. **AlarmService** is started, and alarm sound plays in the background.  
5. User can stop the alarm using **stopService()**.  

---

## 🖼️ Screenshots  


