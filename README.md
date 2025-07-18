# **IOT2050SM-Energy-Data-Management**

- [**IOT2050SM-Energy-Data-Management**](#iot2050sm-energy-data-management)
  - [**Overview**](#overview)
  - [**UCC Production Transparency Campaign**](#ucc-production-transparency-campaign)
    - [**Used Components**](#used-components)
    - [**Goal**](#goal)
    - [**Warning - Hazardous voltage**](#warning---hazardous-voltage)
    - [**Installation and configuration**](#installation-and-configuration)
  - [**Related Links**](#related-links)
  - [**Contribution and Contribution License Agreement**](#contribution-and-contribution-license-agreement)
  - [**Licence and Legal Information**](#licence-and-legal-information)

## **Overview**

This application describes how to collect and manage energy data on an IOT2050SM using a compatible Energy Meter 1238. The performance data will be collected, pre-processed and forwarded to a SCADA system using MQTT.

![Overview](docs/graphics/1-overview.png)

## **UCC Production Transparency Campaign**

The shown Application Example is part of the **UCC Production Transparency Campaign**. The following two-minute video shows the necessary steps as an example.

<video src="docs\videos\iot2050sm-energy-data-management-demo.mp4" controls></video>

### **Used Components**

This Example was created using the following **Software**:

- **On Debian (IOT2050):**
  - Node-Red
  - IOT2050SM WebUI

This Example was created using the following **Hardware**:

- SIMATIC IOT2050SM (6ES7647-0CA00-1AA2)
- SIMATIC SM 1238 Energy Meter 480VAC (6ES7238-5XA32-0XB0)
- 3x ELEQ TQ30 60/1A current transformer

The SCADA part is considered externally in this application example. The necessary hardware and software for this specific example are therefore only listed in part [Data processing in SCADA](docs/README_ScadaData.md). **The primary focus is on data collection, processing and forwarding using the EnergyMeter and IOT2050SM**.

### **Goal**

After working through the following documents, you will know how to:

- Connect and configure an Energy Meter 1238 to the IOT2050SM
- Collect and pre-process energy performance data using Node-Red
- Forward the data to a superior SCADA system using MQTT
- Present and further process the data in SCADA

This documentation will focus on the IOT2050SM part and will only give superficial information about setting up the SCADA system.

### **Warning - Hazardous voltage**

Will cause death or serious injury! This application example requires working with 230V and may only be carried out by qualified personnel.

![warning](docs/graphics/0-voltage-warning.png)

### **Installation and configuration**

Use the following documents for the configuration of the IOT2050SM:

- [Connection and Configuring Energy Meter 1238](docs/README_ConnectingEnergyMeter.md)
- [Data management in NodeRed](docs/README_DataManagementNodeRed.md)
- [Data processing in SCADA](docs/README_ScadaData.md)

## **Related Links**

||Topic|
|-|-|
|1|SIMATIC IOT2050 Forum: [https://sieportal.siemens.com/en-WW/support/forum/topics/309](https://sieportal.siemens.com/en-WW/support/forum/topics/309)|
|2|SIMATIC IOT2050 Download Page: [https://support.industry.siemens.com/cs/document/109741799/downloads-for-simatic-iot20x0](https://support.industry.siemens.com/cs/document/109741799/downloads-for-simatic-iot20x0)|
|3|SIMATIC IOT2050 Guide: [https://sieportal.siemens.com/en-ww/support/forum/posts/IOT2050-Forum-Topics-Overview/332396](https://sieportal.siemens.com/en-ww/support/forum/posts/IOT2050-Forum-Topics-Overview/332396)|
|4|Operating Instructions: [https://support.industry.siemens.com/cs/ww/en/view/109779016](https://support.industry.siemens.com/cs/ww/en/view/109779016)|

## **Contribution and Contribution License Agreement**

Thank you for your interest in contributing. Anybody is free to report bugs, unclear documentation, and other problems regarding this repository in the Issues section.
Additionally everybody is free to propose any changes to this repository using Pull Requests.

If you haven't previously signed the [Siemens Contributor License Agreement](https://cla-assistant.io/industrial-edge/) (CLA), the system will automatically prompt you to do so when you submit your Pull Request. This can be conveniently done through the CLA Assistant's online platform. Once the CLA is signed, your Pull Request will automatically be cleared and made ready for merging if all other test stages succeed.

## **Licence and Legal Information**

Please read the [Legal information](LICENSE.md).
