# GymIOS

GymIOS is a Swift based iOS application that generates fully personalized workout and nutrition plans. The app guides you through account creation, collects your physical information and goals, then uses Google's Gemini models to craft routines and diet suggestions specific to your needs.

## Getting Started
1. **Create an Account** – Enter your name, email, password, and confirm your email isn't already registered. You'll then answer a brief questionnaire about age, height, weight, goal, body structure, workout level, and available workout time.
2. **AI‑Generated Plan** – After submitting the questionnaire the app contacts a remote backend (`Constants.baseURL`) which processes your details with Gemini. You receive a day‑by‑day workout schedule, recommended calories to burn, and a complete nutritional breakdown including protein, carbs, sugars, and water intake.
3. **Sign In** – Once your profile is ready, log in with your email and password. A JWT token is stored securely on device and reused for one week for seamless authentication.

## Features
- **Workout Dashboard** – View your personalized routine, select the day you want to train, and review each exercise with sets, reps, and estimated calories burned.
- **Live Workout Tracking** – Start a workout to display descriptive exercise images and automatic rest timers via iOS live activities and notifications.
- **Nutrition Logging** – Quickly add foods by name or by nutritional values. AI looks up unknown foods and saves them with `PersistenceManager`, while `HealthManager` tracks your calories, protein, carbs, and sugars. Daily values reset automatically at midnight.
- **Progress at a Glance** – Circular progress views show how your consumed nutrients compare to your daily goals, helping you stay on target.
- **Secure Sync** – All profile and workout data is exchanged with the server using JWT‑protected requests, keeping your information safe.

## Screenshots
![image](https://github.com/user-attachments/assets/871892ac-ded1-45d6-a87f-bd7bce5949a5)
![image](https://github.com/user-attachments/assets/17227519-7285-4d65-9dec-28ff6bc50672)
![image](https://github.com/user-attachments/assets/6ca7773b-c59a-4e18-b257-5dd5870fbe9e)
![image](https://github.com/user-attachments/assets/3b329a5e-5d42-4456-a66d-fdfe76f917f3)
![image](https://github.com/user-attachments/assets/863eceba-4a7d-4dbe-bf15-8861dcccec22)
![image](https://github.com/user-attachments/assets/0a37e332-9fd1-4348-be5d-e5fa6ca51904)
![image](https://github.com/user-attachments/assets/98997647-36b1-436a-b79e-19ddac21bb31)
