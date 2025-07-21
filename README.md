# Release Information 

- **Version**: 1.0.0 
- **Certified**: No 
- **Publisher**: Fortinet 
- **Compatible Version**: FortiSOAR 7.4.0 and later 

# Overview 

A campaign targeting SonicWall SMA 100 series appliances is currently under active exploitation, leveraging both known vulnerabilities and potential zero-days to gain persistent access to enterprise networks. The threat actors deploy a custom Linux-based rootkit for stealth and long-term persistence. 

 The **Outbreak Response - SonicWall Secure Mobile Access Attack** solution pack works with the Threat Hunt rules in [Outbreak Response Framework](https://github.com/fortinet-fortisoar/solution-pack-outbreak-response-framework/blob/release/2.1.0/docs/background-information.md#threat-hunt-rules) solution pack to conduct hunts that identify and help investigate potential Indicators of Compromise (IOCs) associated with this vulnerability within operational environments of *FortiSIEM*, *FortiAnalyzer*.

 The [FortiGuard Outbreak Page](https://www.fortiguard.com/outbreak-alert/sonicwall-sma-attack) contains information about the outbreak alert **Outbreak Response - SonicWall Secure Mobile Access Attack**. 

## Background: 

This ongoing campaign was identified by the Google Threat Intelligence Group (GTIG) and has been attributed, with moderate confidence, to a suspected financially motivated threat actor tracked as UNC6148.

Attackers used a mix of known vulnerabilities and likely an unknown (zero-day) flaw to break into these devices. Once inside, they stole admin credentials and one-time password (OTP) data, allowing them to reconnect through VPNs and stay hidden in the network over time even after security updates are installed. This campaign focused on exploiting edge devices as an entry point into company systems. 

A key component of the campaign was the deployment of OVERSTEP, a custom Linux-based rootkit designed for stealth and persistence. Installed on the targeted appliances, OVERSTEP allowed attackers to maintain control, exfiltrate sensitive credentials and certificates, manipulate logs to erase evidence, and initiate outbound communication for command-and-control. 

## Announced: 

Organizations using affected SMA100 appliances should check for potential compromise, rotate credentials, and conduct deep forensic analysis. 

## Latest Developments: 

July 16, 2025: Google Threat Intelligence Group (GTIG) posted a threat blog.
https://cloud.google.com/blog/topics/threat-intelligence/sonicwall-secure-mobile-access-exploitation-overstep-backdoor

May 7, 2025: SonicWall advisory publishedfor CVE-2025-32819, an authenticated file deletion, a vulnerability in SMA100.
https://psirt.global.sonicwall.com/vuln-detail/snwlid-2025-0011

March 12, 2024: SonicWall advisory published for CVE-2024-38475, an unauthenticated path traversal vulnerability in Apache HTTP Server, which affected the SMA 100 series.
https://psirt.global.sonicwall.com/vuln-detail/SNWLID-2024-0018

February 14, 2023: FortiGuard Threat Signal on Ransomware Activities related to DPRK exploiting CVE-2021-20038 (SonicWall SMA100 buffer overflow vulnerability)
https://www.fortiguard.com/threat-signal-report/5017

July 7, 2021: SonicWall advisory published for CVE-2021-20038, an unauthenticated remote code execution.
https://psirt.global.sonicwall.com/vuln-detail/SNWLID-2021-0026 

# Next Steps
 | [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) |
 | -------------------------------------------- | ---------------------------------------------- | ------------------------ | ------------------------------ |