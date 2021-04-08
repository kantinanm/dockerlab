# Docker Codelab  
### Features
Docker codelab with Firebase Hosing  

# How to install
Use powershell or cmd and type by order, please see below.
- `git clone https://github.com/kantinanm/dockerlab.git`
- `cd dockerlab`
    `npm install -g firebase-tools`
    `firebase login --no-localhost`
    - > login to autentication firebase useraccount in your browser.
- > update Your projectId in file .firebaserc on this root project.
  ```javascript
      {
       "projects": {
       "default": "Your projectId"
        }
      }

- > To deploy Please back to root project (dockerlab) and type command below and enter to deploy hosting.
- `firebase deploy --only hosting`

# How to enable emulators
- `firebase init emulators`
-  Which Firebase emulators do you want to set up? Press Space to select emulators, then Enter to confirm your choices.?
 selected -> Hosting Emulator
-  Which port do you want to use for the hosting emulator?
 -> 5000
-  Would you like to download the emulators now? 
 -> Yes

# How to test local
 `firebase emulators:start --only hosting`
-  http://localhost:5000/codelab-1