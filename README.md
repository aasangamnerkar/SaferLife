# SaferLife
Going back to school in the fall and want to trace who you meet? My app uses custom QR codes to trace and monitor everyone you contact in a day. Go back to school safe with SaferLife!

## Inspiration
Last week, I received an email from my school district discussing ways to reopen schools in the fall. They were considering having 1/2 of the students on campus for 1 semester and the other half on the second semester, having teachers move from class to class instead of students, and all other types of scheduling nightmares in order to trace who comes into contact with who. After talking to my parents, I found out that their workplaces were also in a similar state of confusion as to how they could reopen a physical location while keeping track of who contacts who. Later that same day, I opened up Snapchat and noticed how they used a personalized QR code to add users to a personal friends "list." I also realized that almost every student at my school has a mobile device that they carry around all day. At that moment, I got the inspiration to create an app that is able to trace everyone a person comes into contact with via personalized QR codes like Snapchat.
 
## What it does
My app keeps track of the people you come into contact with when you leave the house. It can be used in schools, offices, restaurants, or any public place where you want to keep track of who you meet. Every time you enter a building, room, or meet a person, you find/they show you their individual QR code and you can, like Snapchat, scan it. The app then adds all the person(s) in that room/building (or the individual person you scanned) to your own personal contacted "list" where it monitors if they have COVID/have come into contact with it. (The list only keeps track of people you met in the last 2 weeks). If anyone you have met in the last 2 weeks gets COVID, indirectly through another person/contaminated area or directly face to face, you will be notified that you are at risk of COVID and recommended to self-isolate.
 
## How it helps
 
Without contact tracing, schools and companies are walking blindly into a dangerous situation. They must be able to know who has met who and who is infected with COVID. This app helps them accomplish this goal. School districts, small businesses, and large companies can all use this app to monitor which people their employees/students/customers meet. When the app tells them someone has COVID or is at risk of it, they can ensure no one else meets them in order to prevent others from getting infected.
 
## How it works
I used android studio and Java to create this app. I set up the basic layout with the dashboard, login, and "search" page using the android studio IDE template. I used the Zxing API to scan QR codes and the QRGEncoder API to generate custom QR codes. 
 
How the app works is, after scanning someone's/a location's QR code, it takes all the people that person/location had come into contact with and adds it to your personal list with a time stamp. It monitors all of the people on your list until one of them changes their status to infected. When this happens, the app will notify you, change your status to "At-Risk", and notify all the people on your list that you are potentially infected with COVID and to avoid you.
 
## What's next for QR Contact Tracing
One feature I was working on was using Bluetooth for proximity detection to check if someone is within 6 feet of you. Instead of using QR codes to add people to your contact "list" for one on one meetings, the app would automatically do it on its own and buzz to let you know you have "contacted" someone.
 
##My Challenges
I struggled to make this app initially because I could not figure out how to make a login page for the app. Another issue I had with it was making the QR code scanner work. A large majority of the time developing this app was spent figuring out how to get the custom Zxing camera to display instead of the default android one. 

