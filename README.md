![enter image description here](https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/banner.png?token=GHSAT0AAAAAAB2TICAR6ZT3K4Q2WZFDBRW6Y3JEIDA)
<img src="https://github.com/Education-IT/Game-HelixJump3D/blob/main/images/game.gif?raw=true" alt="Ball jumping" height=655 align="right">

### Final project for the course - ***Mobile Systems Laboratory*** - **UAM** 

> **Completed during the fourth semester of computer science studies.**



The task was to create a mobile application containing specific elements assigned by the instructor. I created a replica of the popular game - **Helix Jump**. I developed my project using **Unity** and the **C#** language. It was my first encounter with this environment. The game only works on Android devices. It includes **notifications** that encourage playing and communicate progress through **achievements**. I also added Unity **banner ads**. The main goal of the game is to overcome obstacles (circles - specifically *red* elements) and reach the *goal* with our character - the *ball*.



![enter image description here](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white) ![enter image description here](https://img.shields.io/badge/Android-3DDC84.svg?style=for-the-badge&logo=Android&logoColor=white) ![enter image description here](https://img.shields.io/badge/blender-%23F5792A.svg?style=for-the-badge&logo=blender&logoColor=white) ![enter image description here](https://img.shields.io/badge/Unity-100000?style=for-the-badge&logo=unity&logoColor=white) [![enter image description here](https://img.shields.io/badge/website-000000?style=for-the-badge&logo=About.me&logoColor=white)](https://education-it.pl/)
### *Helix-Jump Game:*
***Game Menu:***
<ol type="A">
<li>Mute the game.</li>
<li>Exit the application - triggers 3 notifications to encourage returning to the game. They are displayed after 3 seconds, 15 minutes, and 1 hour, respectively.</li>
<li>Change the "skin" of our playing ball. We have 4 options to choose from: soccer ball, apple, onion, and golf ball.</li>
<li>Restart our progress - resets the High Score, level, and ball skin.</li>
<li>Start the game.</li>
</ol>

--------------------------------------
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/changeCharacter.jpg" height=200 align="right">

1. All game elements were created manually using available free tools.
   Circles are **randomly generated** from the "circle base." All 3D objects - Circles / Ball Skins - were also created by me using the **Blender** program.

2. The game starts with the first level, where you have to overcome one obstacle (circle). Each subsequent level follows the same pattern: **level number = number of obstacles**.

---

3. When falling onto a *green* field, the total number of jumps made by our ball (**achievements**) is counted. After each fall, the ball leaves a wet spot whose size is randomly chosen using the `random()` method.

4. When falling onto a *red* field, we lose the game! The "Game Over" screen appears with the option to return to the main menu. A **banner ad** is displayed at the bottom of the screen. Notifications may appear if we have achieved something. During the actual game, the banner ad disappears to avoid irritating the user.

5. When falling onto the last *black circle*, we win and can proceed to the next level. The "victory" screen appears with a banner ad at the bottom of the screen. Notifications may appear if we have achieved something. During the actual game, the banner ad disappears to avoid irritating the user.

<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/addBaner.PNG" align="middle" width="100%">

--------------------------------------

6. When *"flying through"* the hole in the circle, points are counted and added to the `HighScore` variable. The HighScore and level number **do not reset** when exiting the application. After overcoming the circle, it is destroyed and shattered in all directions.

7. During the game, the progress bar and the number of points acquired without "wiping" are visible. The HighScore is only saved when **losing the game**.

8. While in the menu / on the "Game Over" / "win" screen, the ball does not count jumps towards the total jump count (achievements-notifications) even if it bounces.

--------------------------------------

9. New notifications overwrite/delete old, unviewed notifications. This is an anti-spam system, and the currently visible notification contains the most up-to-date information.
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/Notification2.PNG" height=250>

<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/Notification1.PNG" height=200>

----

10. The music has been shortened and looped by me. All sounds are licensed to allow me to make any changes and derive financial benefits from my application.

--------------------------------------

11. The application is stable and does not contain easily detectable errors. I don't notice any in the current version. (Throughout the production stage, I had access to feedback from my testers - partner, sister, and parents. Thanks to them, any errors were identified and promptly fixed.

## Installation:
1. Allow your smartphone to install **"unknown apps"** from **"My Files"** (using `Samsung Galaxy S5 NEO` as an example):
   - Go to **Settings**.
   - Go to **"Biometrics and Security"**.
   - Go to **"Install unknown apps"**.
   - Find **"My Files"** and select **"Allow from this source"**.
2. Download the game `helixjump3D` from my repository.
3. Go to **"My Files"** and search for the downloaded game **"xHelixJump3D"** - then click on its icon and select **"Install"**.
4. The installed game can now be found among other applications.
5. Have fun! 🥇 (The game version in the repository **DOES NOT INCLUDE ADS!** 😃)

## What I Learned:
<img src="https://raw.githubusercontent.com/Education-IT/Game-HelixJump3D/main/images/apple.gif" align="right">

- I had a huge problem with the script that destroyed the overcome circles because I was using the `AddExplosionForce()` method, which caused the ball to accelerate tremendously, resulting in numerous glitches. I searched for solutions for many hours untilI came up with the idea of significantly reducing the weight of those circles from **1** to **0.05**. Thanks to this change, the circles react very strongly to even a microscopic explosion that hardly affects the ball at all. :)
- Although Kotlin and Android Studio were used during the semester for the classes, I challenged myself to create the game using other tools that I was not familiar with. I chose **Unity3D**. It was my first encounter with Unity, Blender, and game development in general. Thanks to this project, I learned a lot about new tools, possibilities, and solutions.
- I spent over **50 hours** creating this project. This time also includes learning the basics of each tool, creating objects and views, and testing the application multiple times. The project exceeded the lecturer's expectations, and I received a score of 750/600 for it.
