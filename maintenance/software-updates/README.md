---
icon: rotate
---

# Software Updates

{% hint style="warning" %}
**#protip** - Verify all Alta X Gen2 components have their software updated together to the latest by referencing the chart below to make sure there are no compatibility issues.
{% endhint %}

## Current Firmware Version

<a href="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/skynode-altaxgen2-v2.3.7-prod.auterionos" class="button primary">DOWNLOAD v2.3.7</a>

<details>

<summary><strong>Alta X Gen2 v2.3.7</strong></summary>

* **Summary**: Feature release bringing a Doodle radio firmware update, thermal mapping features, Pilot Pro RTK improvements, and more
* **Release Date**: September 2026
* **Versions in this package**:
  * Alta X Gen2 Skynode: v2.3.7
  * PX4: v2.3.6
  * AMC: 2.1.0
  * Pilot Pro App: 2.8.6
  * Freefly Updater App: 3.1.2
* **Notes** (Going from Alta X Gen2 v2.2.6 to v2.3.7)
  * **Read more about the highlights** [**here**](https://docs.freeflysystems.com/astro/maintenance/software-release-notes/astro-software-v2.3-whats-new)**.** Astro and Alta X Gen2 share the same v2.3 software release, so the same notes apply.
  * **Flight**
    * **New:** Boom LED feedback during radio pairing.
    * **New:** Pilot Pro kill switch link health check.
    * **New:** Enabled Dual-antenna GNSS heading.
    * **New:** Check for significant disagreement between magnetic and GNSS heading.
    * **New:** Warnings when either GPS module is missing.
    * **Fix:** More permissive in-air GPS checks no longer apply during pre-arm checks.
    * **Fix:** Gimbal tilt-rate zoom scaling no longer applies twice.
    * **Fix:** Drone can no longer initiate failsafe RTL after emergency flight termination.
    * **Fix:** In Manual mode, the arming stick gesture no longer pans the gimbal before takeoff.
    * **Fix:** Switching to automated takeoff immediately after arming in Manual mode no longer skips motor spoolup.
    * **Fix:** Yaw setpoint no longer shifts unexpectedly when switching from Position to Manual mode.
    * **Fix:** Drone no longer maintains vertical velocity too long after switching from Manual to Position mode.
  * **Payload**
    * **Boson Thermal Camera**
      * **New:** FLIR RJPEG image file format support.
      * **New:** Camera multi-capture for missions.
      * **Improvement:** Wildfire preset gamma updated to 1.6.
    * **LR1 Laser Range Finder**
      * **New:** Laser range finder driver installed by default.
        * Blue units can use the LRF add-on without breaking compliance by allowing app installation.
        * **Note:** Uninstall the previously installed `camera-distance-sensor` AOS app to avoid conflicts.
  * **Pilot Pro**
    * **New:** Added a setting to automatically reconnect to an RTK correction source at startup.
    * **Improvement:** Clearer RTK correction status UI.
    * **Improvement:** NTRIP server compatibility, including NTRIP 2.0 casters and chunked data transfer.
    * **New:** Save and load multiple NTRIP server profiles.
    * **New:** Tablet volume raises to 100% when armed and restores when disarmed. Configurable in **Tablet Settings**.
    * **Improvement:** Pilot Pro data interface now reports the active IO mapping configuration, verification status, parameter checksum, app version, and interface version.
    * **Doodle Radio Firmware**
      * **New:** Update Doodle radio firmware to version 2.0 through the Pilot Pro app.
      * **Improvement:** Doodle 2.0 includes bug fixes and improved resilience in heavy RF interference.
  * **Auterion Mission Control**
    * **Improvement:** Base AMC version updated to 1.37.
    * **New:** “Mission Capture Camera” option for multi-camera capture during missions.
    * **Improvement:** Simplified version information in **Vehicle Overview** → **More**.
    * **Improvement:** Manual-mode hover throttle adjustment moved to **Vehicle Overview** → **Flight Config**. It is now shown in normal and advanced modes.
    * **Improvement:** System Health user experience:
      * Standardized vehicle status and health-check severity colors.
        * Red: arming is denied.
        * Orange: arm with caution.
      * **System Health** is now the default panel in **Vehicle Overview**.
      * Added inactive-mode health-check failures to the panel. These result in an orange caution status.
      * Improved several health-check messages.
      * Improved prioritization and deduplication of banner and audible alerts.
      * Disabled audible alerts while disarmed.
    * **New:** Download only new vehicle photos when viewing the gallery.
    * **New:** Button to stop pending downloads while viewing the gallery.
    * **New:** Thermal Next Palette button mapping in normal mode.
    * **New:** Toggle Map/Video button mapping to switch views in the Fly screen.
    * **Improvement:** Firmware compatibility check warns when vehicle firmware is below the minimum compatible version.
    * **New:** LR1 + Boson survey-planning preset.
    * **New:** Pre-filled filename when saving a mission loaded from file.
    * **Improvement:** Removed Acro mode from available flight modes in advanced mode.
    * **Fix:** Parameter files now save with a valid file extension.
    * **Fix:** Parameter files can now be found when loading.
    * **Fix:** All health-check failures are now shown.
    * **Fix:** Health-check failures are shown after failsafe landing from Position Slow mode.
    * **Fix:** Mission flight speed no longer resets when navigating from mission settings.
    * **Fix:** Map tiles now load on iPhone hotspots.
    * **Fix:** Mission flight-speed units now convert correctly.
    * **Fix:** Importing a mission plan now loads mission altitude correctly.
    * **Fix:** Rocker deadband adjustments now apply correctly.
    * **Fix:** The Plan screen is no longer blank after switching from Fly with the camera feed maximized.
    * **Fix:** “Missions do not require Takeoff Item” no longer blocks mission planning.
    * **Fix:** Long-pressing camera zoom buttons now continuously adjusts zoom.
    * **Fix:** The map now centers on the vehicle reliably when it has a GPS position.

</details>

### Latest Versions

<table data-full-width="true" data-search="false"><thead><tr><th width="221">Component</th><th width="248">Current Compatible Versions</th><th width="245">How To Update</th></tr></thead><tbody><tr><td><strong>Alta X Gen2</strong></td><td></td><td></td></tr><tr><td>Software</td><td>2.3.7</td><td><a href="updating-firmware.md#updating-alta-x-gen2-firmware">Alta X Gen2 Firmware</a></td></tr><tr><td><strong>Pilot Pro</strong></td><td></td><td></td></tr><tr><td>Pilot Pro Firmware</td><td>2.2.0</td><td><a href="https://docs.freeflysystems.com/ecosystem/controller/pilot-pro/maintenance/software-and-firmware-updates#how-to-update-pilot-pro-firmware">Update</a> through the Pilot Pro App</td></tr><tr><td>Pilot Pro App</td><td>2.8.6</td><td>Check the <a href="https://docs.freeflysystems.com/ecosystem/controller/pilot-pro/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app</td></tr><tr><td>AMC App</td><td>2.1.0</td><td><p>Check the <a href="https://docs.freeflysystems.com/ecosystem/controller/pilot-pro/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app.</p><p><strong>Desktop downloads:</strong></p><p><a href="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/AuterionMissionControl-amc-v1.37.25-freefly-astro-2.1.0-arm64.dmg">macOS (Apple Silicon)</a></p><p><a href="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/AuterionMissionControl-amc-v1.37.25-freefly-astro-2.1.0.exe">Windows</a></p><p><a href="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/AuterionMissionControl-amc-v1.37.25-freefly-astro-2.1.0-ubuntu.AppImage">Linux</a></p></td></tr><tr><td>Freefly Updater App</td><td>3.1.2</td><td>Check the <a href="https://docs.freeflysystems.com/ecosystem/controller/pilot-pro/maintenance/software-and-firmware-updates#app-updates">"updates"</a> section in Updater app</td></tr><tr><td><strong>Desktop Apps</strong></td><td></td><td></td></tr><tr><td>Freefly PPK App</td><td>1.2.2</td><td><a href="https://docs.freeflysystems.com/ecosystem/workflows/photogrammetry-mapping/ppk-software">Download</a> from the PPK Software page</td></tr><tr><td><strong>Payloads</strong></td><td></td><td></td></tr><tr><td>Freefly Payloads (LR1, A7R4, OGI, Wiris Pro)</td><td><a href="https://docs.freeflysystems.com/ecosystem/payloads/payload-maintenance/gimbal-firmware">See payloads page</a></td><td><a href="https://docs.freeflysystems.com/ecosystem/payloads/payload-maintenance/gimbal-firmware">Gimbal Firmware</a></td></tr></tbody></table>

***

## Previous Firmware Versions

### Alta X Gen2 v2.2 Release Notes

<details>

<summary><strong>Alta X Gen2 v2.2.6</strong></summary>

<a href="https://freeflyeng.s3.us-west-2.amazonaws.com/_SoftwareReleases/skynode-altaxgen2-v2.2.6-prod.auterionos" class="button primary">DOWNLOAD v2.2.6</a>



* **Summary**: New Feature Release. Brings new Boson thermal presets, LR1 and A7R photography improvements, Gremsy VIO plug-and-play, RTK/NTRIP from Pilot Pro, and the rewritten Doodle channel scan.
* **Release Date**: April 2026
* **Versions in this package**:
  * Alta X Gen2 Skynode: v2.2.6
  * AMC: 1.36.24
  * Pilot Pro App: v2.7
  * Gimbal Firmware: v2.3.0
  * Freefly Updater: v3.1.1
  * LR1 Camera Firmware (recommended): v3.0
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

### Alta X Gen2 v2.1 Release Notes

<details>

<summary>Alta X Gen2 v2.1.44</summary>

* **Summary**: First public release of Alta X Gen2 software.
* **Release Date**: January 2026
* **Versions in this package**:
  * Alta X Gen2 Skynode: v2.1.44

</details>
