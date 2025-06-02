# 📷 Depth Camera Driver Setup

> ⚠️ This feature is only available on RobiS models equipped with a depth camera.

---

## 🚀 Start the Depth Camera Driver

Open a new terminal and run the following command:

```bash
roslaunch astra_camera astra_pro_plus.launch
```

This launches the driver for the Orbbec Astra Pro Plus depth camera, initializing the image and depth data streams.

---

## 🖥️ View Image Streams with rqt

To visualize camera outputs including RGB, depth, and IR:

1. Open a **new terminal**
2. Run:

```bash
rosrun rqt_image_view rqt_image_view
```

3. In the GUI that appears, select the desired topic:
   - `/camera/rgb/image_raw`
   - `/camera/depth/image_raw`
   - `/camera/ir/image_raw`

This tool allows you to verify that the camera is publishing all necessary data streams.
   <p align="center">
   <img src="../../imgs/image30.png" alt="button" width="400"/>
   </p>
   <p align="center">
   <img src="../../imgs/image31.png" alt="button" width="400"/>
   </p>
---

> 💡 Tip: If no image appears, ensure that the camera is physically connected and that the driver launch was successful.

Let us know if you'd like to visualize point clouds or use the camera in SLAM/localization tasks!