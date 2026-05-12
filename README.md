# Skiovox v146
A chrome exploit that opens an unblocked chrome window. not tested but could be possible. 

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
6. When you get to the "Network Error" screen, sign into network
