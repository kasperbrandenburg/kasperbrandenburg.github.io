---
layout: post
title: "Autodiscover Open Redirect Vulnerability"
date: 2017-08-21
category: advisories
tags: [CVE-2017-8621, Microsoft, Autodiscover, Open Redirect]
description: >
  Security advisory for Microsoft Autodiscover Open Redirect vulnerability (CVE-2017-8621)
---

## Beskrivelse (Danish)

Du er landet her, fordi din autodiscovery opsætning er sårbar overfor Open Redirect.
Dette kan udnyttes til at skabe phising kampagner eller på andre måde lokke oplysninger ud af medarbejdere.

## English Description

You have arrived here because your autodiscovery configuration is vulnerable to Open Redirect attacks.
This vulnerability can be exploited to create phishing campaigns or otherwise trick information out of employees.

## Technical Details

### Vulnerability Type
- **CVE Reference**: CVE-2017-8621
- **Vulnerability Class**: Open Redirect
- **Affected System**: Microsoft Autodiscover
- **Severity**: Medium to High

### Impact Assessment

The vulnerability allows attackers to:
- Redirect users to malicious websites
- Conduct phishing attacks using trusted domains
- Potentially harvest credentials or sensitive information

## Mitigation Strategies

### Recommended Solutions

Microsoft has provided guidance and patches for this vulnerability:

**Primary Resource**: [Microsoft Security Response Center - CVE-2017-8621](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2017-8621)

### Implementation Steps

1. **Review Configuration**: Audit your current Autodiscover setup
2. **Apply Patches**: Install available security updates
3. **Update Policies**: Implement proper redirect validation
4. **Monitor Traffic**: Watch for suspicious redirect attempts

## Timeline

- **Discovery**: Vulnerability identified in Microsoft Autodiscover
- **Vendor Response**: Microsoft published advisory and mitigation
- **Public Disclosure**: CVE-2017-8621 assigned and published

## References

- [Microsoft Security Response Center](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2017-8621)
- [CVE-2017-8621 Details](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-8621)

---

*This advisory is provided for educational and security improvement purposes.*