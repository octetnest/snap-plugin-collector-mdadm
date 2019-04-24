# snap-plugin-collector-mdadm

This repository contains an mdadm plugin for [Intel's Snap Telemetry Framework](https://github.com/intelsdi-x/snap). The 
structure of this repository has been laid out to reflect the base directory of the appoptics agent, which by default on 
Debian / Ubuntu is `/opt/appoptics`.

## Requirements

* The plugin has been developed for usage with Solarwinds / Appoptics, which is based on Intel's Snap Framework.
* The plugin requires that you install `snap-plugin-lib-py` (`pip install snap-plugin-lib-py`)
* The plugin requires that you give the appoptics user passwordless access to mdadm :

/etc/sudoers.d/appoptics :

```
appoptics ALL=(ALL) NOPASSWD: /sbin/mdadm
```
