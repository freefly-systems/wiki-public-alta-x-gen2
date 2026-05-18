# Software Updates

{% hint style="warning" %}
**#protip** - Verify all Alta X Gen2 components have their software updated together to the latest by referencing the chart below to make sure there are no compatibility issues.
{% endhint %}

## Current Firmware Version

<details>

<summary><strong>Alta X Gen2 v2.2.6</strong></summary>

* **Summary**: New Feature Release. Brings new Boson thermal presets, LR1 and A7R photography improvements, Gremsy VIO plug-and-play, RTK/NTRIP from Pilot Pro, and the rewritten Doodle channel scan.
* **Release Date**: April 2026
* **Versions in this package**:
  * Alta X Gen2 Skynode: v2.2.6
  * AMC: 1.36.24
  * Pilot Pro App: v2.7
  * Gimbal Firmware: v2.3.0
  * Freefly Updater: v3.1.1
  * LR1 Camera Firmware (recommended): v3.0

{% file src="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/skynode-altaxgen2-v2.2.6-prod.auterionos" %}
Download v2.2.6 Firmware
{% endfile %}

* **Notes** (Going from Alta X Gen2 v2.1.x to v2.2.6)
  * **Read more about the highlights** [**here**](https://docs.freeflysystems.com/astro/maintenance/software-release-notes/astro-software-v2.2-whats-new)**.** Astro and Alta X Gen2 share the same v2.2 software release, so the same notes apply.
  * **Flight**
    * **Fix:** Strong magnetic interference warning wording updated for clarity.
  * **Payload**
    * **New:** LR1 and A7R Fixed Focus mode. Locks the camera at the current focus distance without re-racking, ideal after tap-to-focus for near subjects.
    * **Fix:** Blurry Infinity Focus on certain Sigma 24mm lens versions (v.03 firmware). The payload driver now reads lens firmware version and applies the correct focus offset per version, on both LR1 and A7R.
    * **New:** LR1 and A7R RAW and RAW+JPEG image format support. RAW images save to the camera SD card only.
    * **New:** Gremsy VIO is now plug-and-play. Swapping between an LR1 and a VIO no longer requires parameter changes. VIO must be configured correctly or purchased from Freefly. If using VIO geotagging, the MAVLink mode must be changed, which removes the blue configuration of the aircraft.
    * **New:** Boson Wildfire Contrast Preset, pre-configured for wildfire detection with advanced contrast and isotherm defaults.
    * **New:** Simplified Isotherm views for Boson. "Temp Above" and "Temp Below" each expose a single isotherm band, making it easier to highlight the hottest or coldest objects.
    * **New:** Advanced Contrast Settings for Boson are now in a separate dropdown. Switching Contrast Preset resets Advanced Contrast Settings to the new preset's values.
    * **Fix:** Boson radiometric TIFF captures are now significantly faster.
    * **Fix (AMC):** Flir Boson+ 640 added to available camera profiles.
    * **New:** LR1 APS-C crop support in video mode. Requires LR1 camera firmware newer than v1.0.0.
    * **New:** LR1 additional video recording formats, including XAVC S-I 4K.
    * **Fix (AMC):** Flux survey planning improvements.
  * **Pilot Pro**
    * **New:** RTK and NTRIP can now be run from Pilot Pro on MAVLink-over-ethernet vehicles.
    * **New:** Doodle radio channel scan now scores channels by airtime activity, not just noise, with visual bars and per-channel diagnostics.
    * **New:** Customizable Pilot Pro Status page for integrators.
    * **New:** Pilot Pro now always verifies all input-output parameters to ensure the applied config matches controller state.
    * **Improvement:** Android battery optimization configured so critical Freefly apps are not killed when backgrounded.
    * **Improvement:** Graceful tablet shutdown so Android settings persist across boot.
    * **Improvement:** Software update UX.
    * **Improvement:** Better vehicle and serial connection state management.
    * **Fix:** Log pruning is now capped at 3 GB.
    * **Fix (Freefly Updater):** Auto-fetch on app start now works reliably.
    * **New (Freefly Updater):** Pop-up warning when there is no internet connectivity.

</details>

### Latest Versions

<table data-full-width="true"><thead><tr><th width="221">Component</th><th width="248">Current Compatible Versions</th><th width="245">How To Update</th></tr></thead><tbody><tr><td><strong>Alta X Gen2</strong></td><td></td><td></td></tr><tr><td>Software</td><td><strong>2.2</strong>.6</td><td><a href="updating-firmware.md#updating-alta-x-gen2-firmware">Alta X Gen2 Firmware</a></td></tr><tr><td><strong>Pilot Pro</strong></td><td></td><td></td></tr><tr><td>Pilot Pro Firmware</td><td><strong>2.2</strong>.0</td><td><a href="https://freefly.gitbook.io/pilot-pro-public/maintenance/software-and-firmware-updates#how-to-update-pilot-pro-firmware">Update</a> through the Pilot Pro App</td></tr><tr><td>Pilot Pro App</td><td><strong>2.7</strong>.4</td><td>Check the <a href="https://freefly.gitbook.io/pilot-pro-public/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app</td></tr><tr><td>AMC App</td><td><strong>1.36</strong>.24</td><td>Check the <a href="https://freefly.gitbook.io/pilot-pro-public/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app. Desktop versions can be downloaded <a href="https://freeflysystems.com/support/astro-support">here</a>.</td></tr><tr><td>Freefly Updater App</td><td>3.1.1</td><td>Check the <a href="https://freefly.gitbook.io/pilot-pro-public/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app</td></tr><tr><td><strong>Payloads</strong></td><td></td><td></td></tr><tr><td>Freefly Payloads (LR1, A7R4, OGI, Wiris Pro)</td><td><a href="https://docs.freeflysystems.com/ecosystem/payloads/payload-maintenance/gimbal-firmware">See payloads page</a></td><td><a href="https://docs.freeflysystems.com/ecosystem/payloads/payload-maintenance/gimbal-firmware">Gimbal Firmware</a></td></tr></tbody></table>

***

## Previous Firmware Versions

### Alta X Gen2 v2.1 Release Notes

<details>

<summary>Alta X Gen2 v2.1.44</summary>

* **Summary**: First public release of Alta X Gen2 software.
* **Release Date**: January 2026
* **Versions in this package**:
  * Alta X Gen2 Skynode: v2.1.44

</details>
