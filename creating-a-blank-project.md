# Creating a blank project

To install AR Foundation, we need to keep two things in mind:

1. It is a package provided by Unity, so it must be installed through the Package Manager.
2. To use it on a specific platform (iOS, Android, Magic Leap, and/or HoloLens), we must install the corresponding platform modules.

{% embed url="https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@6.2/manual/project-setup/install-arfoundation.html" %}

***

## Installation Options

#### Option 1: Add the packages manually (Preferred)

* Create a project using any 3D template.

<figure><img src=".gitbook/assets/create_blank_project.png" alt=""><figcaption></figcaption></figure>

* From the **Package Manager** window, install the **AR Foundation** package.

<figure><img src=".gitbook/assets/install_arf.png" alt=""><figcaption></figcaption></figure>

* Install the necessary provider plug-ins depending on the platforms you want to develop for using the **Package Manager**, such as AR Core and AR Kit:

<figure><img src=".gitbook/assets/provider_plugin.png" alt=""><figcaption></figcaption></figure>

<div><figure><img src=".gitbook/assets/install-arkit.png" alt=""><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/install-arcore.png" alt=""><figcaption></figcaption></figure></div>

* The last step is to **activate the providers**.

#### Option 2: Use a template

The other alternative is to create a project using the "**AR Mobile**" template:

<figure><img src=".gitbook/assets/ar_template.png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/welcome_template.png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
This option already installs the plugins for us, though we still need to **activate the providers**!
{% endhint %}

***

### Activating the providers

dddRegardless of the option you choose, for each installed module you must enable its plugin provider in the **Player Settings** window, under the **XR Plug-in Management** window:

<figure><img src=".gitbook/assets/android-provider.png" alt=""><figcaption><p>Activating the Android ARCore provider</p></figcaption></figure>

<figure><img src=".gitbook/assets/ios-provider.png" alt=""><figcaption><p>Activating Apple's ARKit provider</p></figcaption></figure>

That same window also indicate us if we need to do some <mark style="background-color:$warning;">**fixes on the project configuration**</mark>, depending on the target platform:

<div><figure><img src=".gitbook/assets/android_fix.png" alt=""><figcaption></figcaption></figure> <figure><img src=".gitbook/assets/apple_fix.png" alt=""><figcaption></figcaption></figure></div>
