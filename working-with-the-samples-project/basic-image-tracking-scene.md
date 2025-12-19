# Basic Image Tracking scene

This scene allows us to understand how we can use ARFoundation to perform one of the most basic AR tracing methods, Image Tracking.

ARFoundation allows us to follow two approaches to set the images:

1. Specifying the pictures at **compile time**, using an [XR Reference Image Library](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.2/manual/features/image-tracking/reference-images.html)
2. Load the pictures at [**runtime**](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.2/manual/features/image-tracking/mutable-libraries.html) (see `DynamicLibrary` component)&#x20;

<figure><img src="../.gitbook/assets/image_libraries.png" alt="" width="375"><figcaption></figcaption></figure>

<div><figure><img src="../.gitbook/assets/image_t_1.gif" alt="" width="563"><figcaption><p>Using a compiled library</p></figcaption></figure> <figure><img src="../.gitbook/assets/image_t_2.gif" alt="" width="563"><figcaption><p>Loading the library at run-time (after pressing the button on the top)</p></figcaption></figure></div>

{% hint style="warning" %}
Unlike Vuforia, we cannot prepare the anchored content inside the Unity editor, but we have to do it using code.&#x20;
{% endhint %}
