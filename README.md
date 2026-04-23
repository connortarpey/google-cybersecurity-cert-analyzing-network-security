# Analyzing network structure and security

Using the NIST Cybersecurity Framework to respond to a security incident. 

## Scenario

You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a denial of service (DoS) attack. 

As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). Use the CSF to help you navigate through the different steps of analyzing this cybersecurity event and integrate your analysis into a general security strategy. We have broken the analysis into different parts in the template below.



# Incident Report Analysis

**Analyst:** Connor Tarpey
**Framework:** NIST Cybersecurity Framework (CSF)

---

## Summary

The company's web services suddenly stopped responding due to an incoming flood of ICMP packets, preventing normal internal traffic from accessing any network resources. Investigation revealed that a malicious actor had sent a flood of ICMP pings through an unconfigured firewall, overwhelming the network in a distributed denial of service (DDoS) attack. The incident response team contained the attack by blocking the incoming ICMP packets and taking all non-critical network services offline so that critical services could be restored.

## Identify

- A malicious actor targeted the company with an ICMP flood attack.
- The entire internal network was affected, and normal traffic could not reach network resources.
- All critical network resources needed to be secured and restored to a functioning state.
- Root cause: an unconfigured firewall that allowed unrestricted ICMP traffic into the network.

## Protect

- Implemented a new firewall rule to limit the rate of incoming ICMP packets.
- Deployed an IDS/IPS system to filter ICMP traffic based on suspicious characteristics.

## Detect

- Configured source IP address verification on the firewall to flag spoofed IP addresses on incoming ICMP packets.
- Implemented network monitoring software to detect abnormal traffic patterns.
- Set up a SIEM for centralized log analysis and network monitoring.

## Respond

For future security events, the cybersecurity team will:

- Isolate affected systems to prevent further disruption.
- Restore any critical systems and services disrupted by the event.
- Analyze network logs for suspicious and abnormal activity.
- Report incidents to upper management and appropriate legal authorities, if applicable.

## Recover

Recovery steps to return network services to a normal functioning state:

1. Block external ICMP flood attacks at the firewall.
2. Stop all non-critical network services to reduce internal network traffic.
3. Restore critical network services first.
4. Once the flood of ICMP packets has timed out, bring all non-critical systems and services back online.

**Long-term improvements:**

- Maintain regular backups.
- Provide security awareness training for employees.
- Use network segmentation to limit the spread of future attacks.
- Keep all systems updated and patched.
