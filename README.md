# Hackintosh-Ryzen-7-3800X-B550M-Plus

only tested on ventura latest

## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **MacPro7,1**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. Boot it! 

## Post install

- Ethernet 
	- Settings -> Network -> Ethernet -> Advenced -> Hardware: Set Configure from Automatically->Manually Then set Speed to 1000baseT, click ok and apply.

	- When firts install, you can set via terminal:

		`ifconfig en0 media 1000baseT`
