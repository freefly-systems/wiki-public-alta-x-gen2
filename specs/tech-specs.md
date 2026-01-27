# Tech Specs

## Propellers

| Material              |     Carbon Fiber Reinforced Nylon |
| --------------------- | --------------------------------: |
| Propeller Orientation |        (2x) CW and (2x) CCW Props |
| Propeller Type        | Folding - 840 x 230 mm (33 x 9in) |

## Battery

| Cells                                                |                                       12S |
| ---------------------------------------------------- | ----------------------------------------: |
| Nominal Battery Voltage                              |                                     44.4V |
| Peak Battery Voltage                                 |                                     50.4V |
| Battery Connectors                                   |                         AS150U Anti Spark |
| Required Minimum Battery Discharge Rating (Per Pack) | 260A per battery (assumes two batteries)  |

{% hint style="warning" %}
Battery hot swaps are not recommended. Please power off the aircraft by disconnecting both batteries when swapping packs to ensure ideal performance and battery lifespan.&#x20;
{% endhint %}

{% hint style="info" %}
More information about the battery, button functions, and status LED indicator codes can be found in the [user manual](https://drive.google.com/file/d/1xZQplgB4Xa2VZYNrqxjLFh52dDPq8ldu/view)
{% endhint %}

Battery Tray Dimensions

![Minimum and Maximum Battery Tray footprint](<../.gitbook/assets/890-00199 Alta X Gen2 Airframe Complete Battery Dims.JPG>)

![Minimum Skyview Battery Tray Footprint](<../.gitbook/assets/Battery Lower Width Min.png>)

![Maximum Skyview Battery Tray Footprint](<../.gitbook/assets/Battery Lower Width Max.png>)

![Maximum Height of Battery for Skyview Mounting](<../.gitbook/assets/Battery Lower Height.png>)

## Weight <a href="#weight" id="weight"></a>

| Maximum Gross Takeoff Weight | 34.9 kg    |
| ---------------------------- | ---------- |
| Maximum Payload              | 15.1 kg    |
| Empty Weight                 | 11.2 kg \* |

\*(0.13 kg heavier than Alta X Gen1 when similarly equipped with payload mounting rails, 5v & 24v regulators, and FPV camera)

## Environmental <a href="#environmental" id="environmental"></a>

| Operating Temperature | -20C to +50C                              |
| --------------------- | ----------------------------------------- |
| Operating Ceiling     | (Weight-dependent. See performance specs) |
| Ingress Protection    | Tested to IP43 equivalent                 |

## Flight Controller

| Flight Controller Hardware | Freefly Custom Designed Skynode                                  |
| -------------------------- | ---------------------------------------------------------------- |
| Flight Controller Software | Auterion Enterprise PX4 (custom for Alta X)                      |
| Mission Control Software   | Auterion Mission Control                                         |
| Online Fleet Management    | Auterion Suite                                                   |
| Flight Modes               | Manual, Altitude Hold, Position Hold, Return, Autonomous Mission |
| Onboard Modules            | Cortex-A53 Computer, LTE                                         |
| Connectivity               | Wifi, USB C, LTE (North America)                                 |
| Supported Radios           | Herelink and Doodle                                              |
| Supported GNSS             | L1/L2 bands for GPS, GLONASS, Beidou and Galileo                 |

## Radio Control

For more information on the Radio, please visit our [Pilot Pro Radio Specs](https://freefly.gitbook.io/pilot-pro-public/specs/radio-technical-specs)

