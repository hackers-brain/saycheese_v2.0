# SayCheese v2.0
![SayCheese v2.0](https://github.com/hackers-brain/saycheese_v2.0/blob/master/saycheese.png)
Developed by Gaurav Raj (Mr. Robot)
Take webcam shots from target just sending a malicious link

# SayCheese v1.1
You can find the original version created by user @thelinuxchoice
here : https://github.com/thelinuxchoice/saycheese
The first version returns some error for me so i modified it

![cheese](https://user-images.githubusercontent.com/34893261/56869077-e5714d80-69d1-11e9-8ce2-29a254021890.jpg)

# How it works?
<p>The tool generates a malicious HTTPS page using Serveo or Ngrok Port Forwarding methods, and a javascript code to cam requests using MediaDevices.getUserMedia. </p>

<p>The MediaDevices.getUserMedia() method prompts the user for permission to use a media input which produces a MediaStream with tracks containing the requested types of media. That stream can include, for example, a video track (produced by either a hardware or virtual video source such as a camera, video recording device, screen sharing service, and so forth), an audio track (similarly, produced by a physical or virtual audio source like a microphone, A/D converter, or the like), and possibly other track types. </p>

[See more about MediaDEvices.getUserMedia() here](https://developer.mozilla.org/en-US/docs/Web/API/MediaDevices/getUserMedia)
<p> To convince the target to grant permissions to access the cam, the page uses a javascript code made by https://github.com/wybiral that turns the favicon into a cam stream.</p>

## Installing (Kali Linux/Termux):

clone this repo
```
git clone https://github.com/hackers-brain/saycheese_v2.0
```
change directory to saycheese_v2.0
```
cd saycheese_v2.0
```
Note : Ngrok should be downloaded and configured with authtoken in order to link link over WAN
        ngrok should be in saycheese_v2.0 folder

now run the script
```
bash saycheese.sh
```
# Credits
**Author : [HackerBrain](https://github.com/hackers-brain/)**

**HackersBrain : [HackTheBox](https://www.hackthebox.eu/profile/303514)**

**HackersBrain : [TryHackMe](https://tryhackme.com/p/hackersbrain)**
