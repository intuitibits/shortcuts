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
* Device Details (Model and iOS version)
* Shortcut Version

**Notes:** 
* This shortcut uses the [https://maclookup.app](https://maclookup.app) API to resolve AP vendor names based on the OUI portion of the BSSID. No BSSID or other information is being shared when calling the API.
* Band information is not directly available from the "Get Network Details" action, so the shortcut uses some heuristics to determine the band based on channel number and Wi-Fi generation (Wi-Fi 4, 5, or 6). If the shortcut cannot determine the band, a "-" is displayed instead.
* Signal quality ratings are based on SNR as follows:

  SNR | Signal Quality
  --- | ---
  Greater than 40 dB   | Excellent
  Between 26 and 40 dB | Good
  Between 16 and 25 dB | Fair
  Between 11 and 15 dB | Poor
  Less than 11 dB      | Very Poor 

### My Cellular

This is a shortcut that generates a report of your cellular connection. It includes the following information:

* Carrier Name
* Radio Technology
* Signal Bars
* Country Code
* Is Roaming Abroad?
* Device Details (Model and iOS version)
* Shortcut Version
