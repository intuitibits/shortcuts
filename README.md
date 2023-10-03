# Shortcuts

In iOS 17, Apple added options to retrieve details about your Wi-Fi and cellular connections via the "Get Network Details" action. We've created a few shortcuts that can be used to access your Wi-Fi and cellular connection details on your iPhone/iPad.

## Requirements

* iOS 17 or higher.

## Install

1. Download and open the shortcut.
2. Choose "+ Add Shortcut" to add the shortcut to your Shortcuts app.
3. [Add the shortcut to your home screen for easy access](https://support.apple.com/guide/shortcuts/add-a-shortcut-to-the-home-screen-apd735880972/ios).

## Shortcuts
### My Wi-Fi

This is a shortcut that generates a report of your Wi-Fi connection. It includes the following information:

* Network Name (SSID)
* Generation
* BSSID
* Channel number
* Band
* Signal (RSSI)
* Noise
* Signal-to-Noise Ratio (SNR)
* Tx and Rx Rates
* Vendor
* IPv4 Address (Local and external)
* IPv6 Address (Local and external)
* MAC Address
* Device Details (Model and iOS version)

**Notes:** 
* This shortcut uses the [https://maclookup.app](https://maclookup.app) API to resolve AP vendor names based on the OUI portion of the BSSID. No BSSID or other information is being shared when calling the API.
* Band information is not directly available from the "Get Network Details" action, so the shortcut uses some heuristics to determine the band based on channel number and Wi-Fi generation (Wi-Fi 4, 5, or 6). If the shortcut cannot determine the band, a "-" is displayed instead.
* Signal quality ratings are based on SNR as follows:

  Signal Quality | SNR
  --- | ---
  Excellent | SNR > 40 dB
  Good | SNR is between 26 and 40 dB
  Fair | SNR is between 16 and 25 dB
  Poor | SNR is between 11 and 15 dB
  Very Poor | SNR <= 10 dB 

### My Cellular

This is a shortcut that generates a report of your cellular connection. It includes the following information:

* Carrier Name
* Radio Technology
* Signal Bars
* Country Code
* Is Roaming Abroad?
* Device Details (Model and iOS version)
