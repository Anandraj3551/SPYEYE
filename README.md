# 📱 **SPYEYE**

### 🔍 **Overview**
This is a camera app that continuously detects objects (bounding boxes and classes) in the frames seen by your device's back camera, using a quantized [MobileNet SSD](https://github.com/tensorflow/models/tree/master/research/object_detection) model trained on the [COCO dataset](http://cocodataset.org/). These instructions walk you through building and running the demo on an Android device.

The model files are downloaded via Gradle scripts when you build and run. You don't need to do any steps to download TFLite models into the project explicitly. 🚀

The application can run either on a physical device or an emulator. 📲

<!-- TODO(b/124116863): Add app screenshot. -->

---

## 🛠️ **Build the Demo using Android Studio**

### ⚙️ **Prerequisites**

* If you don't have it already, install **[Android Studio](https://developer.android.com/studio/index.html)**, following the instructions on the website. 📥

* You need an Android device and Android development environment with a minimum **API 21**. 📱

* Ensure you're using **Android Studio 3.2 or later**. 🖥️

### 🔨 **Building the Demo**

1. Open **Android Studio**, and from the Welcome screen, select **Open an existing Android Studio project**. 📂

2. In the **Open File or Project** window that appears, navigate to and select the `tensorflow-lite/examples/object_detection/android` directory from wherever you cloned the TensorFlow Lite sample GitHub repo. Click **OK**. ✅

3. If it asks you to do a **Gradle Sync**, click **OK**. 🔄

4. You may also need to install various platforms and tools, if you encounter errors like "Failed to find target with hash string 'android-21'" or similar. 📉

5. Click the **Run** button (the green arrow) or select **Run > Run 'android'** from the top menu. 🎯

6. You may need to rebuild the project using **Build > Rebuild Project**. 🔄

7. If it asks you to use **Instant Run**, click **Proceed Without Instant Run**. ⏩

8. Ensure you have an Android device plugged in with **developer options enabled** at this point. See **[here](https://developer.android.com/studio/run/device)** for more details on setting up developer devices. 📱

---

### 🧠 **Model Used**

Downloading, extraction, and placing it in the assets folder has been managed automatically by `download.gradle`. 🔽

If you'd like to explicitly download the model, you can get it from **[here](http://storage.googleapis.com/download.tensorflow.org/models/tflite/coco_ssd_mobilenet_v1_1.0_quant_2018_06_29.zip)**. 🗂️  
Extract the zip to get the `.tflite` and label file.

---

### ⚠️ **Additional Note**

**Please do not delete the assets folder content**. ⚠️  
If you explicitly deleted the files, choose **Build > Rebuild** from the menu to re-download the deleted model files into the assets folder. 🔄

---

Enjoy object detection with your Android device! 🥳📸
