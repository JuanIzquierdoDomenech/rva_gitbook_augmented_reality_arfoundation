# What is AR Foundation?

{% embed url="https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.3/manual/index.html" %}

AR Foundation is Unity’s own solution for developing **Augmented Reality** applications, within the broader framework the platform provides for creating [**Extended Reality (XR)**](https://docs.unity3d.com/6000.2/Documentation/Manual/XR.html) experiences:

* **Augmented Reality (AR)**
* **Virtual Reality (VR)**
* **Mixed Reality (MR)**

<figure><img src=".gitbook/assets/continuum.png" alt=""><figcaption><p>Milgram, Paul, et al. "Augmented reality: A class of displays on the reality-virtuality continuum."</p></figcaption></figure>

Specifically, AR Foundation provides support for developing AR applications on the following platforms:

* **Android**: via **ARCore**
* **iOS**: via **ARKit**
* **visionOS**: for A**pple Vision Pro**
* **HoloLens 2**: using the **OpenXR** Plug-in
* **Meta Quest**: using the **OpenXR** Plug-in
* **Android XR**: using the **OpenXR** Plug-in

***

### Platform Support

The following table summarizes the support for key AR Foundation features across major platforms. This overview focuses on the most widely used and essential capabilities for building cross-platform AR applications.

| **Feature**       | **Android** | **iOS** | **visionOS** | **HoloLens** | **Meta Quest** | **Android XR** | **XR Simulation** |
| ----------------- | ----------- | ------- | ------------ | ------------ | -------------- | -------------- | ----------------- |
| _Session_         | Yes         | Yes     | Yes          | Yes          | Yes            | Yes            | Yes               |
| _Device tracking_ | Yes         | Yes     | Yes          | Yes          | Yes            | Yes            | Yes               |
| _Camera_          | Yes         | Yes     |              | Yes          | Yes            | Yes            | Yes               |
| _Plane detection_ | Yes         | Yes     | Yes          | Yes          | Yes            | Yes            | Yes               |
| _Image tracking_  | Yes         | Yes     | Yes          |              |                |                | Yes               |
| _Face tracking_   | Yes         | Yes     |              |              | Yes            |                |                   |
| _Meshing_         |             | Yes     | Yes          | Yes          | Yes            |                | Yes               |
| _Occlusion_       | Yes         | Yes     |              | Yes          | Yes            | Yes            | Yes               |
| _Raycasts_        | Yes         | Yes     |              | Yes          | Yes            | Yes            | Yes               |
| _Anchors_         | Yes         | Yes     | Yes          | Yes          | Yes            | Yes            | Yes               |

Below are the core features that matter most when designing AR experiences with AR Foundation, explained briefly and clearly.

### Device Tracking

Enables positional and rotational tracking (6DoF).

This is the foundation of all AR experiences: the system must understand where the device is in 3D space to place virtual content accurately.

### Plane Detection

Detects real-world horizontal or vertical surfaces such as floors, walls, or tables.\
Commonly used to:

* Place virtual objects on real surfaces
* Build scenes anchored to the physical world

### Raycasts

Allows the application to intersect a virtual ray with real-world geometry such as planes or meshes.

* Tap-to-place interactions
* Selecting or pointing at surfaces
* Object placement and manipulation

### Anchors

Anchors preserve the position and orientation of virtual objects even when tracking adjustments occur.

* Stable object placement
* Persistent AR content
* Multi-step interactions

### Image Tracking

Recognizes and tracks 2D physical images (posters, cards, logos).

* Marker-based AR
* Print-to-digital interactions
* Trigger-based experiences

### Face Tracking

Detects and tracks human faces with detailed landmarks.

* Masks and face filters
* Avatar interactions
* Expression-driven features

### Meshing

Generates a real-time 3D mesh of the environment.

* Physics interactions with the real world
* Mixed reality occlusion
* Scene understanding

### Occlusion

Allows real-world objects to hide virtual objects, increasing realism.

* Depth-consistent composition
* More immersive placement
* Better integration of virtual objects into the real world
