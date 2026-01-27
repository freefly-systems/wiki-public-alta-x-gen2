# FAQ

#### Does Alta X Gen2 have dual GNSS heading?

* Alta X Gen2 ships with dual onboard F9P GNSS receivers. This currently enables redundancy in case of a single module failure. A future software update will enable dual GNSS aided heading estimation for better performance in degraded conditions.

<br>

#### Does Alta X Gen2 support terrain following?

* Auterion Mission Control has [Digital Elevation/Terrain Model (DEM)](https://www.earthdata.nasa.gov/topics/land-surface/digital-elevation-terrain-model-dem) built into its mission planning features that allow Alta X Gen2 to utilize terrain following during missions.&#x20;
* Alta X Gen2 also includes sensors (laser range finder) to support terrain following, but it is not currently supported in software. We plan to include support for it in a future release.

<br>

#### What power is available onboard?

* Alta X Gen2 includes connectors for unregulated battery power, and regulated 12V and 24V power.
* Accessory battery power is fused at 10A.&#x20;
* 12V power is limited to 10A (120W).
* 24V power is limited to 6.25A (150W).&#x20;

<br>

#### Can I use other batteries with Alta X Gen2?

* Yes, but this requires parameter changes. Alta X Gen2 is designed to use the recommended smart batteries, as these are the most heavily tested and they enable more accurate battery state of charge measurement, but it can be configured to operate on other batteries.
* Note: changing battery modes disables single battery arming prevention. Always use a fused power cable with one battery when powering the aircraft on the ground or bench.&#x20;
* To use XT90 batteries with Alta X Gen2, we offer adapter cables. Contact [Support](https://freeflysystems.com/support) to purchase these.&#x20;
* To change battery modes, see [here](batteries-and-charging.md#switching-battery-modes).

<br>

#### Does Alta X Gen2 include an FPV camera?

* Yes, all variants of Alta X Gen2 include a forward facing NDAA compliant digital FPV camera that streams into AMC on Pilot Pro. &#x20;

<br>

#### Can I use multiple Smart Dovetail payloads?

* Skynode on Alta X Gen2 only supports interfacing to one Smart Dovetail payload at a time. Alta X Gen2 can support multiple payloads if only one is using the Smart Dovetail interface and the others are passive or power only.&#x20;

<br>

#### What’s the max flight time?

* Alta X Gen2’s flight time depends on payload and density altitude. See the performance chart here.

<br>

#### What payloads are supported on Alta X Gen2?

* Alta X Gen2 supports the same payloads as Alta X Gen1, in addition to the following Smart Dovetail payloads. We continue to test new payloads and expand the list of supported payloads.&#x20;
* LR1 Payload
* Wiris Pro Payload
* Gremsy Vio Payload
* Movi Pro / Carbon
* Flux Payload integration is in the works



#### How can I get help?

* Reach out to support by emailing us at support@freeflysystems.com or via our [website](https://freeflysystems.com/contact). Texting or sending social messages will take longer.
*   Share as much detail as possible and provide Alta X Gen2's serial number (located on the rear end of the aircraft by the battery connectors).

    <figure><img src="../.gitbook/assets/image (32).png" alt="" width="563"><figcaption></figcaption></figure>
* Share your flight logs from the Auterion Suite.
* Include photos or videos in your contact in order to get us up to speed as quickly as possible.
* Include pilot statement and notes of any incident or details
