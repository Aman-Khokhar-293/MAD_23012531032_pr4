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
<img width="409" height="906" alt="image" src="https://github.com/user-attachments/assets/9924b1d9-09d5-44dc-a853-7956079efead" />
<br>
<img width="424" height="903" alt="image" src="https://github.com/user-attachments/assets/be5748eb-e7b7-48b6-90b9-920a686d2c68" />
<br>
<img width="415" height="899" alt="image" src="https://github.com/user-attachments/assets/0693115f-a3cb-49ce-971f-704c626c2f9a" />
<br>


