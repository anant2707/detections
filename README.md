# Bluetooth-Based Exfiltration Detection Pack

This repository contains detection logic for identifying potential data exfiltration over Bluetooth using Windows.

## Components

- `sigma/bluetooth_exfiltration.yml`: SIGMA rule for detection logic.
- `sysmon/bluetooth_exfiltration_config.xml`: Minimal Sysmon config to support telemetry needed.

## Usage

1. Deploy Sysmon with the provided config.
2. Ingest logs into your SIEM.
3. Use a Sigma converter (like `sigmac`) to convert rule into Splunk/Elastic/KQL format.

## MITRE ATT&CK Mappings
- T1052.001: Exfiltration Over Bluetooth
- T1112: Registry Modification
- T1056.001: Input Capture – Clipboard
