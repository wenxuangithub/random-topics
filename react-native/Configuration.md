1.	Installed Node.js (node-v16.17.1-x64). 
2.	Open the Command Prompt
3.	Check node.js version 
                node –v
4.	Sign up Expo (https://expo.dev/)
5.	Use npm to install the Expo CLI command line utility:
              npm install -g expo-cli
6.	Check expo version 
               expo -V
7.	Signup expo account, https://expo.dev/signup
8.	Create a new React Native project called "MyMiniProject"
              npx create-expo-app --template 
 
 
npx expo
              cd MyMiniProject
             Cannot find module 'expo/config (optional)
npm i @expo/metro-config  (create metro-config)
Copy and paste metro-config to MyMiniProject
9.	Expo Login by command line (Optional)
              npx expo login
10.	Start "MyMiniProject"
              npx expo
              press w for web debugger
 
              Stop Project
                Ctr + C
           Install web debugger  
npx expo install react-native-web@~0.19.6 react-dom@18.2.0 @expo/webpack-config@^19.0.0       
Start "MyMiniProject"  again
              npx expo 
              press w for web debugger     
11.	Configure Visual Studio Code for React Native Development
Expo Go app for iOS and Android
The fastest way to get up and running is to use the Expo Go app on your iOS or Android device. Expo Go allows you to open up apps that are being served through Expo CLI.
•	Android Play Store - Android Lollipop (5) and greater.
•	iOS App Store - iOS 11 and greater.
When the Expo Go app is finished installing, open it up. If you created an account then you can sign in here on the "Profile" tab. This will make it easier for you to open projects in the client when you have them open in development — they will appear automatically in the "Projects" tab of the client app. 

 


 
12.	Tunneling 
Restrictive network conditions (common for public Wi-Fi), firewalls (common for Windows users), or Emulator misconfiguration can make it difficult to connect a remote device to your dev server over lan/localhost.
Sometimes it's easier to connect to a dev server over a proxy URL that's accessible from any device with internet access, this is referred to as tunneling. expo start provides built-in support for tunneling via ngrok.
             Then run the following to start your dev server from a tunnel URL:
             npx expo start --tunnel
13.	Expo logout by command line
npx expo logout

14.	Configure Visual Studio Code for React Native Development
Format Code with Prettier in Visual Studio Code (https://www.digitalocean.com/community/tutorials/code-formatting-with-prettier-in-visual-studio-code)
•	The Format Document Command
 

•	Automatically Format on Save
 
 

15.	Android emulator (Optional)  (https://www.brainstormcreative.co.uk/react-native-expo/how-to-run-an-expo-app-on-an-android-emulator/)
16.	How to Organize a React Native Project
 


Get Started
https://reactnative.dev/docs/getting-started
https://reactnative.dev/docs/intro-react-native-components
https://reactnative.dev/docs/intro-react
https://docs.expo.dev/tutorial/text/



App.tsx
import { StatusBar } from "expo-status-bar";
import { StyleSheet, Text, View } from "react-native";
import StyleSheets from "./Styles/StyleSheets";

export default function App() {
  return (
    <View style={styles.container}>
      <Text style={{ color: "red", fontSize: 18 }}>
        Open up App.tsx to start working on your app!
      </Text>
      <Text style={styles.bigBlue}>
        Open up App.tsx to start working on your app!
      </Text>
      <Text style={StyleSheets.textColor}>
        Open up App.tsx to start working on your app!
      </Text>
      <StatusBar style="auto" />
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: "#fff",
    alignItems: "center",
    justifyContent: "center",
  },
  bigBlue: {
    color: "blue",
    fontWeight: "bold",
    fontSize: 30,
  },
});
How to Use External Style Sheet in React Native
https://codeflarelimited.com/blog/use-external-style-sheet-in-react-native/

 

StyleSheets.tsx

import { StyleSheet } from 'react-native';


export default StyleSheet.create({
    textColor: {
        color: 'purple',
        fontSize: 50,
    },
});

 
