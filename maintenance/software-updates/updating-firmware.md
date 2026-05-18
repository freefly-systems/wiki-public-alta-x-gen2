# Updating Firmware

## Updating Alta X Gen2 Firmware

{% hint style="info" %}
You can determine if Alta X Gen2 needs an update by following steps 2-4 below. The current firmware version is available on the [Software Updates](./) page.
{% endhint %}

1. Download the firmware from the [Current Firmware Version](./#current-firmware-version) section of the Software Updates page, or from [the Auterion Suite](https://suite.auterion.com/downloads/firmware).
2. Connect Alta X Gen2 to your computer with a USB cable.
3. Power on aircraft **with one battery through the fused cable** and wait about 15 seconds for aircraft to fully boot.
4. Using a browser such as Chrome or Safari, open the aircraft's info/update page at [http://10.41.1.1](http://10.41.1.1/) (internet connection is not needed).
5.  In the Update Auterion OS box, click Browse, and select the firmware file downloaded above.

    <figure><img src="../../.gitbook/assets/image (16).png" alt="" width="563"><figcaption></figcaption></figure>
6. Click Update and wait 10 mins for the process to complete.
7.  After the update completion message, verify that the webpage shows a "Release name" that matches the downloaded file and that all the boom LEDs are on.

    <figure><img src="../../.gitbook/assets/Screenshot from 2026-01-23 12-38-48.png" alt=""><figcaption></figcaption></figure>

If the aircraft gives an error message, power cycle the aircraft and try again.

{% hint style="warning" %}
**If your Alta X Gen2 firmware update fails:**

1. Update the Pilot Pro App to v2.7 or later.
2. Connect Pilot Pro to your Alta X Gen2.
3. Tap the **Fix Me** button in Pilot Pro, which will apply the _FW Updater Fix_. This is found in:\
   &#x20;`App Menu > Vehicle Status Page`&#x20;
4. If you have a Blue/NDAA Alta X Gen2, you will need to disable Admin Protection on the 10.41.1.1/settings page before the _FW Updater Fix_ can apply. Admin Protection can be re-enabled after the firmware update is successful.
5. Retry the Alta X Gen2 firmware update once the _FW Updater Fix_ has been applied.
{% endhint %}

After updating the aircraft, make sure that all apps in the Freefly Updater on Pilot Pro are [up to date](https://freefly.gitbook.io/pilot-pro-public/maintenance/software-and-firmware-updates).

***

## How to Reset to Default Alta X Gen2 Parameters

* Open AMC and activate Advanced mode
* Connect AMC to Alta X Gen2
* Select: Vehicle setup > Parameters > Tools > Reset to vehicle's configuration defaults.
* Reboot Vehicle
* Calibrate sensors as required

<figure><img src="../../.gitbook/assets/Screenshot 2024-03-29 at 12.13.19 PM.png" alt=""><figcaption></figcaption></figure>
