# Release Notes
## Android* Base BSP Reference Release for Intel® Edge Platforms (Intel® Core™ i5 processor 14500T)


Engineering Candidate 1 Release 

February 2026

# 1.0 Introduction

This document provides release specific information about the Android* base BSP reference stack release supported on Intel Edge Platforms (Intel® Core™ i5 processor 14500T) running Android* in a bare-metal OS environment.  

For instructions on building and loading Android* OS on the Intel® Core™ i5 processor 14500T for Edge Platforms, refer to the Android* OS on Intel® Core™ i5 processor 14500T for Edge Platforms Getting Started Guide (Published in [GitHub](https://github.com/edge-aosp-bsp/manifest/blob/master/Getting_Started.md)).

    
> **Note**
> This release is intended for testing and evaluation on the platform
only. It is not for production use.

# Terminology

| Term                     | Description                                                     |
|--------------------------|-----------------------------------------------------------------|
| ADB                      | Android Debug Bridge                                            |
| AOSP                     | Android Open Source Project                                     |
| AVB                      | Android Verified Boot                                           |
| BSP                      | Board Support Package                                           |
| CODEC                    | Coder‑Decoder                                                   |
| CRB                      | Customer Reference Board                                        |
| DP                       | DisplayPort                                                     |
| EC                       | Engineering Candidate                                           |
| HDMI                     | High‑Definition Multimedia Interface                            |
| IFWI                     | Integrated Firmware Image                                       |
| ISV                      | Independent Software Vendor                                     |
| NVME                     | Non‑Volatile Memory Express                                     |
| RDC                      | Resource and Documentation Center                     |
| RVP                      | Reference Validation Platform                     |


## Intended Audience

This document is intended for OSVs/ISVs interested in using Android\* on
Intel® Core™ i5 processor 14500T for Edge Platforms to enable their
customers.

## Customer Support

Contact your Intel representative for support or submit an issue to
[premiersupport.intel.com](http://premiersupport.intel.com/).

## Reference Documents

| Documentation on GitHub | Document No./Location |
|---------|------------------------|
| Android* base BSP Reference Release for Intel® Edge Platforms (Intel® Core™ i5 processor 14500T) – Get started guide |  [GitHub](https://github.com/edge-aosp-bsp/manifest/blob/master/Getting_Started.md) |
| Raptor Lake‑S Refresh Android Manifest File | [GitHub](https://github.com/edge-aosp-bsp/manifest/blob/master/stable-build/A16/BM_BSP_2026_Q1_v1_A16.xml) |

Log in to the Resource and Documentation Center
([rdc.intel.com](https://www.intel.com/content/www/us/en/resources-documentation/developer.html))
to search for and download the document numbers listed in the following
table. Contact your Intel field representative for access.

> **Note**
> Third-party links are provided as a reference only. Intel does not control or audit third-party benchmark data or the websites referenced in this document. You should visit the referenced website and confirm whether the referenced data are accurate. 


| Documentation on Intel RDC | Document No./Location |
|---------|------------------------|
| 13th Gen Intel® Core™ Processors and Intel® Core™ Processors (14th Gen) (Code named Raptor Lake‑S/S Refresh) for Edge Platforms Reference UEFI BIOS/IFWI Version 6311_00 – IFWI Release Notes & Package |  [865275](https://www.intel.com/content/www/us/en/secure/content-details/865275/content-details.html) |



# 2.0 Best-Known Configuration

This section shows the compatible hardware and software configuration for this release.  


## Hardware Configuration

1. **RVP**: SR14 Raptor Lake‑S RVP

2. **Silicon**: QS / PRQ Silicon
   - Intel® Core™ i5 processor 14500T

---

## Software Configuration

1. EC1 Manifest File: [GitHub - BM_BSP_2026_Q1_V1_A16.xml](https://github.com/edge-aosp-bsp/manifest/blob/master/stable-build/A16/BM_BSP_2026_Q1_v1_A16.xml)

2. UEFI Reference BIOS:
   - Release Notes & Package [865275](https://www.intel.com/content/www/us/en/secure/content-details/865275/content-details.html)


# 3.0	Components

This section contains general release information for BSP.


## Release Information

| Type             | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| Release Version  | Engineering Candidate 1 (EC1)                                               |
| Build Target     | caas-userdebug<br>caas-user                                                 |
| Tested Hardware  | SR14 Raptor Lake‑S DDR5 UDIMM 1DPC RVP &<br>Q37X Intel® Core™ i5 processor 14500T |
| Android Version  | android‑16.0.0                                                              |
| Kernel Version   | 6.12.63                                                                     |

## Product Features

## List of Product Features

| Feature Category | Feature                         | Availability |
|------------------|----------------------------------|--------------|
| Connectivity     | Intel Wi‑Fi* 6 & 7    | Yes          |
|                  | Bluetooth® 5.3 & 5.4                      | Yes          |
| ADB              | ADB over Ethernet               | Yes          |
| Media            | Video playback                  | Yes          |
| Display          | eDP                            | Yes          |
|                  | DP over USB‑Type C         | Yes          | 
|                  | Dual Display                | Yes          |
| Audio            | Audio – Onboard CODEC           | Yes          |
|                  | Audio – USB 3.1                 | Yes          |
|                  | Audio – USB‑C                   | Yes          |
|                  | Audio – Bluetooth®              | Yes          |
| USB              | USB‑C                           | Yes          |
|                  | USB 3.2                         | Yes          |
|                  | USB 2.0                         | Yes          |
| Ethernet         | Ethernet                        | Yes          |
| I/O         | USB                        | Yes          |
|          | Serial Port                       | Yes          |
| Storage          | NVMe                            | Yes          |
| Touch            | eDP Touch              | Yes          |
| Camera           | USB                             | Yes          |
| Boot           | Fast Boot / Secure Boot / AVB                             | Yes          |
| OTA           | OTA Enabled                             | Yes          |


# Known Issues

| Issue ID | Feature                         |
|------------------|----------------------------------|
|NIACP3-1149 | Display brightness control is not functional on eDP   |     
|NIACP3-1168 | Error while trying to read the reboot reason while Android boots UP                 |  
|NIACP3-1148 |Screen flicker observed on Type-C touch display| 



# Disclaimer

You may not use or facilitate the use of this document in connection
with any infringement or other legal analysis concerning Intel products
described herein. You agree to grant Intel a non-exclusive, royalty-free
license to any patent claim thereafter drafted which includes subject
matter disclosed herein.

No license (express or implied, by estoppel or otherwise) to any
intellectual property rights is granted by this document.

All information provided here is subject to change without notice.
Contact your Intel representative to obtain the latest Intel product
specifications and roadmaps.

The products described may contain design defects or errors known as
errata which may cause the product to deviate from published
specifications. Current characterized errata are available on request.

Copies of documents which have an order number and are referenced in
this document may be obtained by calling 1-800-548-4725 or visiting the
[Intel Resource and Documentation
Center](https://www.intel.com/content/www/us/en/resources-documentation/developer.html).

Intel technologies\' features and benefits depend on system
configuration and may require enabled hardware, software or service
activation. Performance varies depending on system configuration. No
product or component can be absolutely secure. Check with your system
manufacturer or retailer or learn more at
[intel.com](http://intel.com/).

The Bluetooth® word mark and logos are registered trademarks owned by
Bluetooth SIG, Inc. and any use of such marks by Intel Corporation is
under license.

© Intel Corporation. Intel, the Intel logo, and other Intel marks are
trademarks of Intel Corporation or its subsidiaries. Other names and
brands may be claimed as the property of others.








