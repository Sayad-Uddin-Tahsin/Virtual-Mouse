# Virtual-Mouse
Virtual-Mouse is a mouse that brings functionalities of a regular mouse to your PC camera.  It brings the convenience of moving cursor and clicking functionalities just by showing hand gestures to your camera.

You need a camera/webcam set up with your PC.

## How to use?
It's very simple. When all is `OK` and pops up a window showing the camera window. Show your hand, you will see 2 circles in 2 dedicated fingers `Thumb` & `Index Finger` in the camera view.

##
**Q:** How can I move my mouse cursor?

**A:** ___It's Simple! Just move your `Index Finger` to move your cursor!___

##
**Q:** How can I click to a button or on something?

**A:** ___It's also really simple! All you need to touch your `Index Finger` with your `Thumb` or just need to make the distance between `Index` and `Thumb` Fingers minimum `20` pixels!___

##
 **Tip:** You can also change the minimum distance by changing `20` here: https://github.com/Sayad-Uddin-Tahsin/Virtual-Mouse/blob/62db0a2c5f3587b97188fc24788f02e537c637cb/main.py#L37
 
## Names of Fingers
 ![Names of Fingers](https://image.shutterstock.com/image-vector/fingers-names-human-body-parts-260nw-1042963189.jpg)
 

## Software Requirements
- [Python](https://python.org)
- An IDE for editing code:
   - [Pycharm Communit Edition](https://www.jetbrains.com/pycharm/download)
   - [Visual Studio Code](https://code.visualstudio.com/download)
   - [Spyder](https://www.spyder-ide.org/#section-download)
   - others...

## Module Requirements
| Module | Version | `pip` Command |
| :--: | :-----: | :---: |
| msvc-runtime | 14.29.30133 | `pip install msvc-runtime==14.29.30133` |
| opencv-python | 4.6.0.66 | `pip install opencv-python==4.6.0.66` |
| mediapipe | 0.8.10 | `pip install mediapipe==0.8.10` |
| PyAutoGUI | 0.9.53 | `pip install pyautogui==0.9.53` |

## Problems

Some predicted Problems with Solutions mentioned down there!

##
### Mediapipe
**Error:**

`ImportError: DLL load failed while importing _framework_bindings: The specified module could not be found.`

**Solve:**

For the module `msvc-runtime` this error should be fixed. If it not, please install [Microsoft Visual C++](https://docs.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170). If you have that in your PC, please consider installing the updated [Microsoft Visual C++](https://docs.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist?view=msvc-170). If you get that error after installing, please Restart your PC!

##
### opencv-python(cv2)
**Error:**

`ConnectionAbortedError: cv2: No Camera Found!`

**Solve:**

This error occurs, when the program can't find your Camera. It usually appears when you use more than one camera! You have to specify a single camera by changing the camera number here: https://github.com/Sayad-Uddin-Tahsin/Virtual-Mouse/blob/62db0a2c5f3587b97188fc24788f02e537c637cb/main.py#L5 I used `0` here because there is a single camera in my PC! You can try changing it to `1` or `2`!
