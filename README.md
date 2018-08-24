Pasos:

#plantilla blank que trae ionic
ionic start demo blank --cordova

cd demo

#verificar si toma las plataforms, en caso contrario seguir con los pasos, despues volver a este
ionic cordova plataform add android
ionic cordova plataform add ios

#Para integrar Google Maps Nativo de ionic, necesitaremos hacer uso del plugin de Google Maps.
ionic cordova plugin add cordova-plugin-googlemaps --variable API_KEY_FOR_ANDROID="YOUR_ANDROID_API_KEY_IS_HERE" --variable API_KEY_FOR_IOS="YOUR_IOS_API_KEY_IS_HERE" --save
npm install @ionic-native/google-maps --save

#verificar que se instalen bien los plugin.....

#Prueba de fuego
npm install

#si esta todo ok hasta este paso hacer
sudo ionic cordova run android

#ese ultimo paso va a depender si tienen los skd, jdk y el avd instalado en forma correcta.
