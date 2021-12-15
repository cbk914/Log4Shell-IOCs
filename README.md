# Log4Shell-IOCs

Members of the Curated Intelligence Trust Group have compiled a list of IOC feeds and threat reports focused on the recent Log4Shell exploit targeting CVE-2021-44228 in Log4j

#### Analyst Comments:

- 2021-12-13
  - IOCs shared by these feeds are `LOW-TO-MEDIUM CONFIDENCE` we strongly recommend `NOT` adding them to a blocklist
  - These could potentially be used for `THREAT HUNTING` and could be added to a `WATCHLIST`
  - Curated Intel members at various organisations recommend to `FOCUS ON POST-EXPLOITATION ACTIVITY` by threats leveraging Log4Shell (ex. threat actors, botnets)
  - IOCs include JNDI requests (LDAP, but also DNS and RMI), cryptominers, DDoS bots, as well as Meterpreter or Cobalt Strike
  - Critical IOCs to monitor also include attacks using DNS-based exfiltration of environment variables (e.g. keys or tokens) - see [here](https://twitter.com/captainGeech42/status/1470055184449613829)
- 2021-12-14
  - Curated Intel members profiled active exploitation threats
- 2021-12-15
  - Curated Intel members parsed `MEDIUM CONFIDENCE FEEDS` to be `MISP COMPATIBLE` using [KPMG's MISP implementation](https://github.com/curated-intel/Log4Shell-IOCs/tree/main/Threat%20Hunt%20Feed%20-%20Medium%20Confidence)

### `Indicators of Compromise (IOCs)`
| Source | URL |
| --- | --- |
| GreyNoise (1) | https://gist.github.com/gnremy/c546c7911d5f876f263309d7161a7217 |
| Malwar3Ninja's GitHub | https://github.com/Malwar3Ninja/Exploitation-of-Log4j2-CVE-2021-44228/blob/main/Threatview.io-log4j2-IOC-list |
| Tweetfeed.live by @0xDanielLopez | https://twitter.com/0xdaniellopez/status/1470029308152487940?s=21 |
| Azure Sentinel | https://raw.githubusercontent.com/Azure/Azure-Sentinel/master/Sample%20Data/Feeds/Log4j_IOC_List.csv |
| URLhaus | https://urlhaus.abuse.ch/browse/tag/log4j/ |
| Malware Bazaar | https://bazaar.abuse.ch/browse/tag/log4j/ |
| ThreatFox | https://threatfox.abuse.ch/browse/tag/log4j/ |
| Cronup | https://github.com/CronUp/Malware-IOCs/blob/main/2021-12-11_Log4Shell_Botnets |
| RedDrip7 | https://github.com/RedDrip7/Log4Shell_CVE-2021-44228_related_attacks_IOCs |
| AbuseIPDB | `Google/Bing Dorks`  site:abuseipdb.com "log4j", site:abuseipdb.com "log4shell", site:abuseipdb.com "jndi" |
| CrowdSec | https://gist.github.com/blotus/f87ed46718bfdc634c9081110d243166 |
| Andrew Grealy, CTCI | https://docs.google.com/spreadsheets/d/e/2PACX-1vT1hFu_VlZazvc_xsNvXK2GJbPBCDvhgjfCTbNHJoP6ySFu05sIN09neV73tr-oYm8lo42qI_Y0whNB/pubhtml# |
| Bad Packets | https://twitter.com/bad_packets/status/1469225135504650240 |
| NCSC-NL | https://github.com/NCSC-NL/log4shell/tree/main/iocs |
| Costin Raiu, Kaspersky | https://twitter.com/craiu/status/1470341085734051840?s=21 |
| Kaspersky | https://securelist.com/cve-2021-44228-vulnerability-in-apache-log4j-library/105210/ |
| SANS Internet Storm Center | https://isc.sans.edu/diary/Log4Shell+exploited+to+implant+coin+miners/28124 |
| @cyber__sloth | https://twitter.com/cyber__sloth/status/1470353289866850305?s=21 |
| SuperDuckToes | https://gist.github.com/superducktoes/9b742f7b44c71b4a0d19790228ce85d8 |
| Nozomi Networks | https://www.nozominetworks.com/blog/critical-log4shell-apache-log4j-zero-day-attack-analysis/ |
| Miguel Jiménez | https://hominido.medium.com/iocs-para-log4shell-rce-0-day-cve-2021-44228-98019dd06f35 |
| CERT Italy | https://cert-agid.gov.it/download/log4shell-iocs.txt |
| RISKIQ | https://community.riskiq.com/article/57abbfcf/indicators |
| Infoblox | https://blogs.infoblox.com/cyber-threat-intelligence/cyber-campaign-briefs/log4j-exploit-harvesting/ |

### `Threat Reports`

| Source | Threat | URL |
| --- | --- | --- |
| @GelosSnake | Kinsing | https://twitter.com/GelosSnake/status/1469341429541576715 |
| @an0n_r0| Kinsing | https://twitter.com/an0n_r0/status/1469420399662350336?s=20 |
| @zom3y3 | Muhstik | https://twitter.com/zom3y3/status/1469508032887414784 |
| 360 NetLab (1) | Mirai, Muhstik | https://blog.netlab.360.com/threat-alert-log4j-vulnerability-has-been-adopted-by-two-linux-botnets/ |
| MSTIC (1) | Cobalt Strike | https://www.microsoft.com/security/blog/2021/12/11/guidance-for-preventing-detecting-and-hunting-for-cve-2021-44228-log4j-2-exploitation/ |
| Cronup | Kinsing, Katana-Mirai, Tsunami-Muhstik | https://twitter.com/1zrr4h/status/1469734728827904002?s=21 |
| Cisco Talos | Kinsing, Mirai | https://blog.talosintelligence.com/2021/12/apache-log4j-rce-vulnerability.html |
| Profero | Kinsing | https://medium.com/proferosec-osm/log4shell-massive-kinsing-deployment-9aea3cf1612d |
| CERT.ch | Kinsing, Mirai, Tsunami | https://www.govcert.ch/blog/zero-day-exploit-targeting-popular-java-library-log4j/ |
| IronNet | Mirai, Cobalt Strike | https://www.ironnet.com/blog/log4j-new-software-supply-chain-vulnerability-unfolding-as-this-holidays-cyber-nightmare |
| @80vul | New Ransomware | https://twitter.com/80vul/status/1470272820571963392 |
| @Laughing_Mantis | Log4j Worm | https://twitter.com/Laughing_Mantis/status/1470168079137067008 |
| Lacework | Kinsing, Mirai | https://www.lacework.com/blog/lacework-labs-identifies-log4j-attackers/ |
| 360 NetLab (2) | Muhstik, Mirai, BillGates (Elknot), XMRig, m8220, SitesLoader, Meterpreter | https://blog.netlab.360.com/ten-families-of-malicious-samples-are-spreading-using-the-log4j2-vulnerability-now/ |
| Trend Micro | Cobalt Strike, Kirabash, Swrort, Kinsing, Mirai | https://www.trendmicro.com/en_us/research/21/l/patch-now-apache-log4j-vulnerability-called-log4shell-being-acti.html |
| BitDefender | Khonsari Ransomware, Orcus RAT, XMRig, Muhstik | https://businessinsights.bitdefender.com/technical-advisory-zero-day-critical-vulnerability-in-log4j2-exploited-in-the-wild |
| MSTIC (2) | PHOSPHORUS, HAFNIUM, Initial Access Brokers | https://www.microsoft.com/security/blog/2021/12/11/guidance-for-preventing-detecting-and-hunting-for-cve-2021-44228-log4j-2-exploitation/ |
| Cado Security (1) | Mirai, Muhstik, Kinsing | https://www.cadosecurity.com/analysis-of-initial-in-the-wild-attacks-exploiting-log4shell-log4j-cve-2021-44228/ |
| Cado Security (2) | Khonsari Ransomware | https://www.cadosecurity.com/analysis-of-novel-khonsari-ransomware-deployed-by-the-log4shell-vulnerability/ |
| Valtix | Kinsing, Zgrab | https://valtix.com/blog/log4shell-observations/ |
| Fastly | Gafgyt | https://www.fastly.com/blog/new-data-and-insights-into-log4shell-attacks-cve-2021-44228 |

### `Payload Examples`

| Source | URL |
| --- | --- |
| GreyNoise (2) | https://gist.github.com/nathanqthai/01808c569903f41a52e7e7b575caa890 |
| Cloudflare | https://blog.cloudflare.com/actual-cve-2021-44228-payloads-captured-in-the-wild/ |
| yt0ng | https://gist.github.com/yt0ng/8a87f4328c8c6cde327406ef11e68726 |
| eromang | https://github.com/eromang/researches/tree/main/CVE-2021-44228 |
| VX-Underground | https://samples.vx-underground.org/samples/Families/Log4J%20Malware/ |
| Malware-Traffic-Analysis (PCAP) | https://www.malware-traffic-analysis.net/2021/12/14/index.html |
| rwincey| https://github.com/rwincey/CVE-2021-44228-Log4j-Payloads |

### `Threat Profiling`
| Threat                | Type                             | Profile: Malpedia                                                                                                    | Profile: MITRE ATT&CK                                                                     | Activity                                                                                                                                                   |
| --------------------- | -------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Cobalt Strike         | Attack tool usage                | [Cobalt Strike (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/win.cobalt_strike) | [Cobalt Strike, Software S0154 | MITRE ATT&CK®](https://attack.mitre.org/software/S0154/) | [Command and Control, Tactic TA0011 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/tactics/TA0011/)                                                |
| Orcus RAT             | Attack tool usage                | [Orcus RAT (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/win.orcus_rat)         | N/A                                                                                       | [Command and Control, Tactic TA0011 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/tactics/TA0011/)                                                |
| Meterperter           | Attack tool usage                | [Meterpreter (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/win.meterpreter)     | N/A                                                                                       | [Command and Control, Tactic TA0011 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/tactics/TA0011/)                                                |
| BillGates / Elknot    | Botnet expansion (DDoS)          | [BillGates (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/win.billgates)         | N/A                                                                                       | [Acquire Infrastructure: Botnet, Sub-technique T1583.005 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1583/005/)                     |
| Mirai (AKA Katana)    | Botnet expansion (DDoS, miner)   | [Mirai (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/elf.mirai)                 | N/A                                                                                       | [Acquire Infrastructure: Botnet, Sub-technique T1583.005 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1583/005/)                     |
| Muhstik (AKA Tsunami) | Botnet expansion (DDoS, miner)   | [Tsunami (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/elf.tsunami)             | N/A                                                                                       | [Resource Hijacking, Technique T1496 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1496/)                                             |
| Kinsing               | Botnet expansion (miner)         | [Kinsing (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/elf.kinsing)             | [Kinsing, Software S0599 | MITRE ATT&CK®](https://attack.mitre.org/software/S0599/)       | [Resource Hijacking, Technique T1496 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1496/)                                             |
| m8220                 | Botnet expansion (miner)         | N/A                                                                                                                  | N/A                                                                                       | [Resource Hijacking, Technique T1496 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1496/)                                             |
| Swrort                | Downloader usage (stager)        | [Swrort Stager (Malware Family) (fraunhofer.de)](https://malpedia.caad.fkie.fraunhofer.de/details/ps1.swrort)        | N/A                                                                                       | Ingress Tool Transfer, Technique T1105 - Enterprise | MITRE ATT&CK®                                                                                        |
| SitesLoader           | Downloader usage (stager)        | N/A                                                                                                                  | N/A                                                                                       | [Ingress Tool Transfer, Technique T1105 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1105/)                                          |
| Kirabash              | Infostealer usage                | N/A                                                                                                                  | N/A                                                                                       | [OS Credential Dumping: /etc/passwd and /etc/shadow, Sub-technique T1003.008 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1003/008/) |
| XMRig                 | Mining tool usage                | N/A                                                                                                                  | N/A                                                                                       | [Resource Hijacking, Technique T1496 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1496/)                                             |
| New Ransomware        | Ransomware usage                 | N/A                                                                                                                  | N/A                                                                                       | [Data Encrypted for Impact, Technique T1486 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1486/)                                      |
| Khonsari Ransomware   | Ransomware usage                 | N/A                                                                                                                  | N/A                                                                                       | [Data Encrypted for Impact, Technique T1486 - Enterprise | MITRE ATT&CK®](https://attack.mitre.org/techniques/T1486/)                                      |
