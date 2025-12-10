Wazuh SIEM Enhancement & Detection Experiments

A structured project for SIEM improvement and detection engineering with the focus of integrating new log sources, validation of telemetry ingestion, and conducting controlled adversary simulation with Windows Defender and Atomic Red Team.



This sprint expands an existing Wazuh SIEM deployment by adding Windows Defender telemetry from the ad01 Windows Server, enabling richer endpoint visibility and more realistic SOC-style monitoring. It also brings in several detection experiments mapped to MITRE ATT&CK to assess the coverage of SIEM and validate alerting.



Integrate Windows Defender logs into Wazuh to track malware detections, scan activity, configuration changes, and endpoint protection events.

It used the EICAR test file to validate the successful ingestion of malware detection logs and confirm SIEM-to-endpoint visibility.

Executed Atomic Red Team – T1548.002 to test the SIEM detection capability for privilege escalation techniques.

Monitored indicators included suspicious process creation, parent-child anomalies, and eventvwr.exe exploitation attempts.

Conducted Defender-based experiments on:

Manual full system scans

Scanning results and action logging

Temporary disabling of AV settings to simulate attacker tampering

Verified what events Wazuh captured, and documented logging gaps for future tuning.


Tools & Frameworks

Wazuh SIEM

Windows Defender AV telemetry

Atomic Red Team - T1548.002 Bypass UAC

MITRE ATT&CK framework

Sysinternals ProcMon

Windows Event Logs



This project demonstrates practical skills in:

Onboarding and enrichment of SIEM logs

Detection engineering

MITRE ATT&CK Mapping

Endpoint security monitoring

Security Experiment Design and Validation



Stephen Ettienne
Security+ Certified | Cybersecurity Analyst 
