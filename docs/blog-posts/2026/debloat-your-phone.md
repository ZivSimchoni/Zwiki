---
title: Debloat Your Android Device Without Root - Using Shizuku, Hail & Canta.
---

# Debloat Your Android Device Without Root

Most Android phones ship with a bunch of pre-installed apps you never asked for, don't want and probably never use such as carrier apps, manufacturer "extras", duplicate apps, spyware, bloatware and so on.<br>
These apps spy on you, waste storage, consume battery in the background and clutter your app drawer.<br>
The good news? You can get rid of them **without rooting your phone** (at least most of them).

This guide walks you through debloating your Android device using **Shizuku**, **Hail** and **Canta**.

!!! warning "Proceed with caution"
    Removing the wrong system app can cause unexpected behavior or even a boot loop. **Always research an app before uninstalling it.** When in doubt, _freeze_ or _disable_ instead of _uninstalling_.

---

## What You'll Need

- An Android phone (for obvious reasons).
- Approx. 10 minutes of your time.

## Tools Overview

| Tool | What It Does |
| :--- | :----------- |
| [Shizuku](https://shizuku.rikka.app/) or [thedjchi's Shizuku Fork](https://github.com/thedjchi/Shizuku) | Grants ADB-level privileges to apps on your phone, so you don't need a PC connected every time. |
| [Hail](https://github.com/aistra0528/Hail/blob/master/README_EN.md) | A simple app that uses Shizuku to freeze apps. |
| [Canta](https://github.com/samolego/Canta) | A simple app that uses Shizuku to uninstall/disable bloatware with a few taps. |

---

## Common Bloatware Safe to Remove

!!! danger "Do **NOT** remove core system apps like Phone, Settings, SystemUI, or anything related to Google Play Services (unless you know exactly what you're doing and/or are replacing them with alternatives)."

Experiment with the app/s by freezing/uninstalling them one by one and checking if your phone still works as expected, sometimes it wont. In case something isnt working as you expected, you can always **unfreeze**/**restore** the app.

Here are some apps that are _generally_ safe to remove on most devices (always verify for your specific phone model):

- Carrier-specific apps (e.g. T-Mobile, Vodafone, carrier billing apps)
- Manufacturer duplicate apps (e.g. Samsung Browser, Samsung Email, Mi Video)
- Pre-installed social media apps (e.g. Facebook, LinkedIn, Netflix)
- Demo or promotional apps
- Apps that are not needed for the phone to function properly (Easter eggs, Test apps for the factory, etc.)

## Step 1 — Setup Shizuku

!!! tip "After daily driving OG Shizuku for a while, I now use the thedjchi's fork since it provides me with the ability to start Shizuku's service automatically without any further interaction. and it is more stable for me."

Install Shizuku and setup the service by following [Shizuku's Docs](https://shizuku.rikka.app/guide/setup/#start-via-wireless-debugging).

## Step 2 - Install & Use Hail

1. Install [Hail](https://github.com/aistra0528/Hail/blob/master/README_EN.md) ([F-Droid Link](https://f-droid.org/packages/com.github.hail_dev.hail/)).
2. Open Hail — it will ask for Shizuku permission. Tap **Allow**.
3. Navigate to the `Apps` tab, select the app/s you want to freeze.
4. In the `Home` tab, you can see a list of apps that you have selected to be frozen. (BTW you can `tag` apps to have more control over what you freeze).

## Step 3 — Install & Use Canta

1. Install [Canta](https://github.com/samolego/Canta) ([F-Droid Link](https://f-droid.org/packages/org.samo_lansen.canta/)).
2. Open Canta — it will ask for Shizuku permission. Tap **Allow**.
3. In the top right corner there is a `Filter` icon, select **Reccomended** to see a list of apps that are generally safe to remove.

!!! tip "Canta has a community-maintained bloatware list that labels apps as safe or unsafe to remove. Use it as a starting point but always double check before uninstalling."

## Personal take  

If im not sure about an app my flow is usually as follows:

1. I search online for the app's package name to see if an app is safe to remove or not for my specific phone model. (I usually trust [Reddit](https://www.reddit.com/) and [XDA-Developers](https://forum.xda-developers.com/)).
2. I use Hail to freeze the app and see if my phone still works as expected.
3. If my phone still works as expected, I use Canta to uninstall the app.
4. Some apps may "restore" themselves after an software update (OTA). In that case I usually freeze them instead of uninstalling them. (e,g., Samsung Game Optimization Service)

## Summary

| Step | Action |
| :--: | :----- |
| 1 | Enable Developer Options & USB Debugging |
| 2 | Install Shizuku & start it via ADB |
| 3 | Install Hail, grant Shizuku permission & freeze bloatware (Recommended for apps you are **not sure** about).|
| 4 | Install Canta, grant Shizuku permission & uninstall bloatware (Recommended for apps you are **sure** about).|

Once Shizuku is running, Hail and Canta are set up, debloating is as easy as selecting apps and tapping **freeze/uninstall** — **no root, no terminal commands**.

??? question "Questions about this post"
    *Have you debloated your phone before? What method did you use?<br>
    * Did this guide help? Is there anything that could be clearer?<br><br>
    Please let me know, any feedback is appreciated!  
