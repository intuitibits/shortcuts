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
* RSSI
* Noise
* SNR
* Tx and Rx Rates
* Vendor
* Local IPv4 Address
* Local IPv6 Address
* MAC Address
* Device Details (Model and iOS version)

**Note:** This shortcut uses the [https://maclookup.app](https://maclookup.app) API to resolve AP vendor names based on the OUI portion of the BSSID. No BSSID or other information is being shared when calling the API.

### My Cellular

This is a shortcut that generates a report of your cellular connection. It includes the following information:

* Carrier Name
* Radio Technology
* Signal Bars
* Country Code
* Is Roaming Abroad?
* Device Details (Model and iOS version)
