---
name: MSc - ORB-SLAM and COLMAP
tools: [Python, COLMAP, ORB-SLAM2]
image: ../UniPictures/SLAM.png
description: Comparing ORB-SLAM2 and COLMAP for monocular visual SLAM and reconstruction quality benchmarking.
---

# ORB-SLAM2 and COLMAP

This module focused on gaining familiarity with **visual SLAM systems**, specifically **ORB-SLAM2** and **COLMAP**, with an emphasis on **monocular SLAM**. The primary objective was to collect and evaluate small datasets that demonstrate both the strengths and limitations of ORB-SLAM2, while using COLMAP reconstructions as a **ground truth reference** for comparison.

To investigate performance, various **camera settings (frame rate, resolution, and exposure)** were tested to determine how these parameters affect reconstruction quality and robustness.

---

## Outdoor Track Sequence

The first experiment involved walking around a **running track**, a scene expected to be ideal for SLAM due to its simple path and open visibility. However, the low visual diversity — repetitive colours, distant trees, and few unique features — caused **ORB-SLAM2 to fail completely**, unable to maintain sufficient feature tracking.  
In contrast, **COLMAP** successfully completed the reconstruction, highlighting its ability to exploit **high-resolution imagery** to identify and match subtle scene features.

<div style="text-align: center; margin: 2rem 0;">
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 900px; margin: auto;">
    <iframe
      src="https://www.youtube.com/embed/n_AQjk6trv8?autoplay=1&mute=1&loop=1&playlist=n_AQjk6trv8&controls=0"
      title="Outdoor Track Sequence"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
    </iframe>
  </div>
</div>

---

## Indoor Navigation Sequence

The second test took place in an **indoor university setting**, where the goal was to create a controlled environment with known feature points. Initially, both systems struggled due to **low texture areas** and **large frame-to-frame movements**. To improve results, we manually **increased scene texture** by placing magazines, objects, and pool balls within the environment.  
We also **mounted the camera on a wheeled chair** for smoother motion, reducing motion blur and frame jumps. These adjustments led to excellent reconstructions for both ORB-SLAM2 and COLMAP, producing **accurate, consistent maps** with strong feature correspondence.

<div style="text-align: center; margin: 2rem 0;">
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 900px; margin: auto;">
    <iframe
      src="https://www.youtube.com/embed/BA8RjpVHJLY?autoplay=1&mute=1&loop=1&playlist=BA8RjpVHJLY&controls=0"
      title="Indoor Navigation Sequence"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
    </iframe>
  </div>
</div>

---

## Outdoor Driving Sequence

Finally, a **KITTI-style driving dataset** was captured by mounting a stabilized camera to a car roof and driving through a suburban neighbourhood.  
This test showcased **ORB-SLAM2’s strongest performance**, maintaining stable feature tracking despite objects moving both toward and across the camera’s field of view. The distinct geometry and texture of the environment (buildings, road markings, and vehicles) produced a **clean, high-quality reconstruction**.

<div style="text-align: center; margin: 2rem 0;">
  <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 900px; margin: auto;">
    <iframe
      src="https://www.youtube.com/embed/c6kvqg2iobs?autoplay=1&mute=1&loop=1&playlist=c6kvqg2iobs&controls=0"
      title="Outdoor Car Sequence"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
      allowfullscreen
      style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;">
    </iframe>
  </div>
</div>

---

### 💡 Key Takeaways

- Gained hands-on experience with **ORB-SLAM2** and **COLMAP** for monocular visual SLAM.  
- Conducted experiments comparing **frame rate, resolution, and environmental texture** on reconstruction quality.  
- Discovered the strengths of COLMAP in static high-resolution contexts versus ORB-SLAM2’s real-time adaptability.  
- Learned to **capture and prepare datasets** suitable for benchmarking SLAM performance.  

---

{% include elements/button.html 
    text="<i class='fas fa-file-download'></i> GitHub Link"
    size="sm"
    link="https://github.com/WillTerry01/COMP2049-SLAM/tree/main/Coursework2"
%}
