# Reference

This is a list of all the methods available on the tramontana object in Processing. 

###### Actuators


Haptics
[makeVibrate()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#makeVibrate--)

Media
[showImage(String url)
](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#showImage-java.lang.String-)[playAudio(String url)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#playAudio-java.lang.String-)
[playVideo(String url)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#playVideo-java.lang.String-)
*`loopVideo(String url)`*

Flash light
[setFlashLight(float onValue)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#setFlashLight-float-)
[pulseFlashLight(int numberOfPulses, float duration, float intensity)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#pulseFlashLight-int-float-float-)

Screen
[setBrightness(float brightness)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#setBrightness-float-)
[setColor(float red, float green, float blue, float intensity)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#setColor-float-float-float-float-)
[setColor(int red, int green, int blue, int intensity)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#setColor-int-int-int-int-)
[transitionColors(float r1, float g1, float b1, float a1, float r2, float g2, float b2, float a2, float duration)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#transitionColors-float-float-float-float-float-float-float-float-float-)




###### Subscribe - Sensors

[subscribeAttitude()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeAttitude--)
[subscribeAttitude(int frequency)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeAttitude-int-)
[subscribeAudioJack()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeAudioJack--)
[subscribeDistance()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeDistance--)
[subscribeMagnetometer()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeMagnetometer--)
[subscribeOrientation()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeOrientation--)
[subscribePowerSource()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribePowerSource--)
[subscribeTouch()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeTouch--)
[subscribeTouch(Boolean multitouch)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeTouch-java.lang.Boolean-)
[subscribeTouchDrag()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeTouchDrag--)
[subscribeTouchDrag(Boolean multitouch)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#subscribeTouchDrag-java.lang.Boolean-)

###### Callback methods 

*`onVideoEndEvent(String ipAddress)
onAttitudeEvent(String ipAddress, float yaw, float pitch, float roll)
onAudioJackEvent(String ipAddress, int isIn)
onMagnetometerEvent(String ipAddress, int isAboveThreshold, float magnetometerValue)
onDistanceEvent(String ipAddress, int distanceValue)
onOrientationEvent(String ipAddress, int orientation)
onPowerSourceEvent(String ipAddress, int orientation)
onTouchEvent(String ipAddress, int x,int y)
onTouchDragEvent(String ipAddress, int x,int y)
onTouchDownEvent(String ipAddress, int x,int y)
onMultiTouchEvent(String ipAddress, ArrayList touches, int numTouches)
onMultiTouchDragEvent(String ipAddress, ArrayList touches, int numTouches)
onMultiTouchDownEvent(String ipAddress, ArrayList touches, int numTouches)
gotBatteryUpdate(String ipAddress, float batteryValue)`*


###### Camera
[takePicture()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#takePicture--)
[takePicture(int camera)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#takePicture-int-)
[takePictureWithUI(int camera)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#takePictureWithUI-int-)


###### Embedded Actuators

*`setServoEmbedded(int servoIndex, int value)
setRelayEmbeddedOff(int relayIndex)
setRelayEmbeddedOn(int relayIndex)
sendSerialMessageEmbedded(String msg)
setColorEmbedded(int ledIndex,int red, int green, int blue)
blinkColorEmbedded(int ledIndex,int red, int green, int blue)
setAllColorEmbedded(int red, int green, int blue)`*

###### Embedded Sensors

*`subscribeRxEmbedded()
releaseRxEmbedded()
subscribeButtonsEventEmbedded()
releaseButtonsEventEmbedded()
subscribeAnalogEmbedded()
releaseAnalogEmbedded()
subscribeLDREmbedded()
releaseLDREmbedded()`*

###### Embedded Callbacks
*`onEmbeddedBtnsEvent(String ip, int btnIndex, int btnValue)
onEmbeddedRxEvent(String ip,String msg)
onEmbeddedAnalogUpdate(String ip, int value)
onEmbeddedLDRUpdate(String ip, int value)`*

###### Utilities

[version()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#version--)
[getBatteryLevel()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#getBatteryLevel--)

###### OSC - Machine Learning

[sendAttitudeDataToOSC(float frequency, int port)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#sendAttitudeDataToOSC-float-int-)
[sendAttitudeDataToOSC(float frequency, int port, String ip)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#sendAttitudeDataToOSC-float-int-java.lang.String-)
[sendTouchDataToOSC(int maxNumFingers)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#sendTouchDataToOSC-int-)
[sendTouchDataToOSC(int maxNumFingers, int port)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#sendTouchDataToOSC-int-int-)
[sendTouchDataToOSC(int maxNumFingers, int port, String ip)](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#sendTouchDataToOSC-int-int-java.lang.String-)
[stopAttitudeDataToOSC()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#stopAttitudeDataToOSC--)
[stopTouchDataToOSC()](https://pierdr.github.io/Tramontana-for-Processing/reference/tramontana/library/Tramontana.html#stopTouchDataToOSC--)


