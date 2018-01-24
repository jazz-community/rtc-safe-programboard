# rtc-safe-programboard
do distributed SAFe PI Planning or Scrum-of-Scrums Big Room Planning with a virtual board in RTC

![SAFeProgramBoardRTC](docs/images/SAFeProgramBoardRTC.jpg)

## Information and latest News
- [Blog on wordpress.com](https://timeboxplanning.wordpress.com/)
- [YouTube Channel](https://www.youtube.com/channel/UCcvclkdfdmOS6AuR62bZ_PA/playlists)
- [Presentation on slideshare.net](https://www.slideshare.net/MarkusGiacomuzzi)

## Idea and goal
This extension delivers a virtual and highly customizable SAFe Program Board similar to the one proposed by SAFe
The widget is available as a serverside plugin, which can be installed on any RTC (CCM) instance.

## Compatibility
The Widget works for CLM V.4.0.3 and later. Currently it is in successful operation on V.6.0.5.
Since it is implemented process independently it supports the brand new IBM SAFe template as well as any others including your customizations

## Releases
Today we offer you a binary distribution, which can be downloaded from this project and installed on your system. The current stable release can be downloaded directly from the [Releases](https://github.com/jazz-community/rtc-safe-programboard/releases) page.

## Installation
Deploy just like any other update site:

1. Extract the `com.siemens.bt.jazz.programboard.v1_updatesite.ini` **file** from the zip file to the `server/conf/ccm/provision_profiles` directory
2. Extract the `com.siemens.bt.jazz.programboard.v1_updatesite` **folder** to the `server/conf/ccm/sites` directory
3. Restart the server

## Update existing installation
1. Request a server reset in one of the following ways:
    * If the server is currently running, call `https://server-address/ccm/admin/cmd/requestReset`
    * Navigate to `https://localhost:9443/ccm/admin?internaltools=true` so you can see the internal tools (on the left in the side-pane). Click on `Server Reset` and press the `Request Server Reset` button
    * If your server is down, you can delete the ccm `built-on.txt` file. Liberty packed with 6.0.3 puts this file in a subfolder of `server/liberty/servers/clm/workarea/org.eclipse.osgi/**/ccm`. The easiest way to locate the file is using your operating system's search capabilites.
2. Delete previously deployed updatesite folder
3. Follow the file extraction steps from the section above
4. Restart the server

## Contributing
Please use the [Issue Tracker](https://github.com/jazz-community/rtc-safe-programboard/issues) of this repository to report issues or suggest enhancements.
Please refer to our [Contributing Guide](CONTRIBUTING.md#contributing) if you would like to help us improving this software.

## Licensing
Copyright (c) Siemens AG. All rights reserved.<br>
Licensed under the [MIT](LICENSE.md) License.

