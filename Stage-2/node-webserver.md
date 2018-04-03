How is everyone running their servers? I'm currently using python simpleHTTPServer but I'm having some issues with it. Does anyone have an easy alternative? I'm not very good with setting up servers


15 replies
MHD [23 hours ago]
first of all check your python version with `python -v`

chose the correct command to run your server depending on your python version, two or three. 

make sure when you execute this command that you are in the project root directory


MHD [23 hours ago]
@Jennah let me know if you need more info (edited)


Jennah [23 hours ago]
@MHD I've been using python server for the majority of the project. But I want to try something different now due to problems...  I'm pretty sure it's not a problem with my code as everything was working yesterday. Thank you for the tips though


MHD [23 hours ago]
@Jennah
maybe this could help ? 
https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en
chrome.google.com
Web Server for Chrome
A Web Server for Chrome, serves web pages from a local folder over the network, using HTTP. Runs offline.
 


Jennah [23 hours ago]
@MHD thanks, I'll have a look :slightly_smiling_face:

nicolas [23 hours ago]
I recommend you try npm's `serve` package.

```// to install
npm i -g serve

// then to open at port 8000 and auto open a browser for you
serve -p 8000 -o```
 


Jennah [23 hours ago]
@nicolas thank you!! My project is working again! :slightly_smiling_face:


nicolas [23 hours ago]
No worries :slightly_smiling_face:

JeremieL [19 hours ago]
Hi @nicolas, always awesome to read about inputs! Do you need to run `npm i -g serve` into the repo directory? 

EDIT: yes of course; I need to be in the repo folder! :wink: (edited)


nicolas [19 hours ago]
@JeremieL I guess you found out by yourself :wink:


nicolas [18 hours ago]
@JeremieL It doesn't matter where you run `npm i -g serve` as this will install the `serve` library globally, making it available wherever you are. What does matter is that you start your server calling `serve` in the repo folder you want to use as a server.


nicolas [18 hours ago]
Adding to this, you only need to run `npm i -g serve` once. After that, the library is installed and from that moment onwards you will just need to call it whenever you wish to open up a local server.


nicolas [18 hours ago]
And you can run `serve -h` to see some further options you have when initialising your server.


JeremieL [18 hours ago]
Cool stuff. I am really excited to learn more about node and npm tricks :slightly_smiling_face: Great to have you on this track!



nicolas [18 hours ago]
Btw, `npm i -g <package-name>` is short for `npm install --global <package-name>`, expanding just to avoid confusion. (edited)
