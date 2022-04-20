# Introduction

Azure IoT Hub onboarding guide for TPM protected device.

# Table of Contents

- **[Prerequisites](#prerequisites)**
- **[Guide](#guide)**
- **[References](#references)**
- **[License](#license)**

# Prerequisites

- Raspberry Pi 4 Model B
- Iridium 9670 TPM 2.0 board [[2]](#2)

# Guide

Azure IoT Hub:
<table>
<tr>
    <th>Device Type</th>
    <th colspan="4">Authentication Type</th>
</tr>
<tr>
    <th></th>
    <th>Symmetric key</th>
    <th>X.509 Self-Signed</th>
    <th>X.509 CA Signed</th>
</tr>
<tr>
    <td align="center">Ordinary <a href="#3">[3]</a></td>
    <td align="center"><a href="docs/1.md">1.md</a></td>
    <td align="center"><a href="docs/2.md">2.md</a></td>
    <td align="center"><a href="docs/3.md">3.md</a></td>
</tr>
<tr>
    <td align="center">Edge <a href="#4">[4]</a></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>
<tr>
    <td align="center">Leaf <a href="#5">[5]</a></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>
</table>

Azure IoT Hub Device Provisioning Service:
<table>
<tr>
    <th>Device Type</th>
    <th colspan="4">Attestation Mechanism</th>
</tr>
<tr>
    <th></th>
    <th>Symmetric key</th>
    <th>X.509 Self-Signed</th>
    <th>X.509 CA Signed</th>
    <th>TPM</th>
</tr>
<tr>
    <td align="center">Ordinary <a href="#3">[3]</a></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"><a href="docs/4.md">4.md</a></td>
</tr>
<tr>
    <td align="center">Edge <a href="#4">[4]</a></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>
<tr>
    <td align="center">Leaf <a href="#5">[5]</a></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
    <td align="center"></td>
</tr>
</table>
<!--
DPS - indi enrollment - ordinary device - symmetric keys - ?: https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-symm-key
DPS - indi enrollment - ordinary device - X.509 - ?: https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509
DPS - group enrollment - ordinary device - symmetric keys - soft key: https://docs.microsoft.com/en-us/azure/iot-dps/how-to-legacy-device-symm-key
DPS - group enrollment - ordinary device - X.509  - soft key: https://docs.microsoft.com/en-us/azure/iot-dps/tutorial-custom-hsm-enrollment-group-x509
-->

# References

<a id="1">[1] https://www.infineon.com/cms/en/product/security-smart-card-solutions/optiga-embedded-security-solutions/optiga-tpm/</a> <br>
<a id="2">[2] https://www.infineon.com/cms/en/product/evaluation-boards/iridium9670-tpm2.0-linux/</a> <br>
<a id="3">[3] https://docs.microsoft.com/en-us/azure/iot-fundamentals/iot-glossary#device</a> <br>
<a id="4">[4] https://docs.microsoft.com/en-us/azure/iot-fundamentals/iot-glossary#leaf-device</a> <br>
<a id="5">[5] https://docs.microsoft.com/en-us/azure/iot-fundamentals/iot-glossary#iot-edge-device</a> <br>

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

