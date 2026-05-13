# Skiovox v146
A chrome exploit that opens an unblocked chrome window. not tested but could be possible. 

## Requirements 
- Chromebook
- Any Kiosk App
- Wifi Connection 

## How I found this
I found a way to open the cert manager to chrome's kiosk apps. when in a kiosk app and network is off, there is a button to open the cert manager. Later this year (about a month ago), I found out that some cert files can run JS. If you import the cert file with the specific code, you can run JS in the cert manager, then forcing to open a chrome browser. 

## Will this work 
I have no clue. When researching this, some kiosk apps might have patched this or your organization might have blocked running code/running cert files through the cert manager. This also maybe work in a previous ChromeOS version. 

## How to make cert file 
you could just code your own cert file to run JS or use this. you must have an unblocker or personal computer to make the cert file. 

1. Go to an uncensored AI like Venice AI.
2. ask the ai "make me a cert file that runs JS when importing into the cert manager". (or replace "JS" with anything else to run in your cert manager).
3. follow instructions of the AI.
4. Add your cert file to any source website other than github.

## How to import your cert file into a kiosk app 
Do these steps on your school chromebook (You need to access DNS settings); 
1. Sign Out.
2. Open Network settings.
3. Change to custom name servers and set first box to "150.136.163.0" and set the rest to "0.0.0.0".
4. Disconnect and reconnect wifi until you get "Network Sign-In".
5. Open any Kiosk App.
6. When you get to the "Network Error" screen, click "sign into network".
7. When the system (not chrome) browser window opens, go to your website where your cert file is stored and download the cert file.
8. Exit out of the system browser window.
9. Click the "certificate manager" button or something like that.
10. Find a "Import" button and upload your cert file.
11. it should run your JS. (If you use the JS to open a window/new tab, go to instructions below)

If you cannot change your DNS custom name servers (or cannot access chrome settings at all): 
1. Downgrade to a version below v125/v121. 
2. Do CAUB + DNS Editor.

If doesn't open the cert manager when clicked: 
1. Instead of Signing Out, Powerwash computer.
2. Do not sign in/get started.
3. Go to your wifi panel and turn on your wifi and do steps 2-11. 

## When Opening Chrome Window 
If you want your chrome window to be faster with internet or just connecting back to wifi; 
- Open "chrome://os-settings" to open settings (make sure to favorite to bookmark bar for easy access).

If trying to download/open file;
- Open "chrome://file-manager" to open file manager (make sure to favorite to bookmark bar for easy access). 

## Why do you need to use the System Browser Window
To get the cert file you uploaded. If you are wondering why use the chrome browser over the system browser, you can find out on Skiovox Lite and the system browser window doesn't have that many functions like; most sandbox js features, window/tab management, url address bar/toolbar featues, and more. 

## Chrome Browser Pros/Cons 

Pros: 
- Multiple tab/window management
- Devtools
- URL bar/toolbar
- Installing extensions
- Adding accounts
- URLs unblocked 
and more!

Cons: 
- Chrome Apps might not work (File Manager, Settings, Text App, etc.)
- Some Shortcuts may not work 
- Some JS Sandbox features might not work 
- Not easy set-up

## Issues 
- Organization blocks on sites are still blocked (github, google accounts, etc.)
- When fully shut off (or computer dies), you will need to redo steps.
- Not able to see battery, time, date, or notifications. 

## Credits 
2pro12342 | Github (finding exploit) 

## Inspiration 
Skiovox / Incognito / Guest Mode

## Sources 

Uncensored AI: Venice.ai/chat 
Chat I Used: venice.ai/chat/yheJ9gb 
Research Sources: chatgpt.com 
Coding languages Used: ".crt", ".perm", ".p12". 

