# MISP — Threat Intelligence Platform

## Overview

This project documents my hands-on experience deploying and exploring MISP (Malware Information Sharing Platform), an open-source threat intelligence platform, in my home SOC lab.

I practised reviewing threat intelligence events, exploring indicators of compromise (IOCs), and understanding how threat intelligence supports security alert investigation.

MISP is the threat intelligence layer in a SOC stack. When an alert fires, analysts can look up observables such as IP addresses, hashes, and domains in MISP to gain context and identify potentially related indicators or campaigns. This helps turn isolated alerts into better-informed investigations.

## Lab Setup

- **Platform:** MISP
- **Deployment:** Docker using misp-docker
- **Environment:** Ubuntu virtual machine
- **MISP URL:** `https://192.168.56.102:8080` (local lab address)
- **Threat intelligence source:** CIRCL OSINT Feed (Computer Incident Response Center Luxembourg)
- **Events displayed in the lab:** 1,681-event count observed during the lab session

## What I Practised

- Threat feed ingestion and event browsing
- Exploring event attributes such as IP addresses, domains, URLs, and file hashes
- Understanding attribute types, categories, and tags
- Learning how related indicators can help analysts investigate suspicious activity
- Understanding how MISP can support SIEM alert enrichment and incident response

## Resource Management

My home lab has limited virtual machine memory, so I run MISP when needed and stop its containers when the work is complete to free resources for other SOC tools.

## Screenshots

**Events list from the MISP lab**

![MISP events list](screenshots/misp_events_populated.png)

**Event detail and attributes**

![MISP event detail with attributes](screenshots/misp_event_detail.png)

## Future Improvements

- Explore MISP integration with TheHive for observable enrichment
- Investigate additional threat intelligence feeds
- Practise enriching simulated SOC alerts using threat intelligence

## Disclaimer

This is a learning project conducted in a personal home lab. The screenshots document the MISP interface and event data available in my lab; they do not represent an investigation of a live security incident.
