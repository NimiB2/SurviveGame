# APK Game Project

This project is a study assignment where I reverse-engineered an APK file, analyzed its code, and recreated the app in Android Studio. Below is a detailed explanation of what I did, the challenges I faced, and how the game works.

![sol](https://github.com/user-attachments/assets/31010482-46c3-4638-855d-44bcc92bdeb5)


## What I Did

1. **Extracting the APK Files:**
   - I downloaded the APK file and renamed it to a `.zip` file.
   - I used Windows Shell to extract the contents of the APK after downloading it from the APK decompiler website.

2. **Creating a New Project:**
   - I started a new Android Studio project.
   - In the extracted APK folders, I found the relevant `Activity` files and copied them one by one into my project.
   - I also copied the corresponding XML files for these activities into my project.

3. **Completing Missing Resources:**
   - After adding the activities and XML files, I noticed some `drawable` files were missing.
   - I searched for these missing files and added them to my project to complete the resources.

4. **Fixing Issues:**
   - I encountered a small error with a `Toast` message. I debugged it and fixed the issue.
   - When I ran the app, I found another issue: the URL in the code had invisible characters that caused it to lead to the wrong website. I removed these characters, fixed the URL, and the game worked.

## How the Game Works

1. **Starting the Game:**
   - The game starts by asking the user to input an ID number (a series of digits).

2. **Processing the ID:**
   - Each digit in the ID is divided by 4, and the remainder (a number between 0-3) is calculated.
   - Each remainder represents a direction in the game:
     - `0` = Right
     - `1` = Left
     - `2` = Up
     - `3` = Down

3. **Game Logic:**
   - The order of the remainders represents the sequence of directions the user needs to follow.
   - By following the correct sequence, the user unlocks the city name from the URL that the app processes.

## Challenges I Faced

- **Finding Missing Resources:** I had to carefully analyze the project to identify missing drawable files and manually add them.
- **Fixing Code Errors:** I debugged a small issue in a `Toast` message.
- **Correcting the URL:** The URL in the code contained invisible characters that led to the wrong site. I removed the characters and fixed the issue.

## Summary

This project helped me learn how to decompile an APK, analyze its components, and recreate a functional version of the app. I also gained experience in debugging and resolving resource issues.

---
