# DDOS Attack - Volumetric

Amplified reflection attacks are a type of [DDoS attack](https://www.a10networks.com/blog/what-is-a-ddos-attack/) that exploits the connectionless nature of UDPs with spoofed requests to misconfigured open servers on the internet. Amplified reflection attacks take the prize when it comes to the size of the attack.

The attack sends a volume of small requests with the spoofed victim’s IP address to accessible servers. The servers reply with large amplified responses to the unwitting victim. The servers can do this because they are configured with services that the attackers sought out for their ability to aid in this attack.

[https://youtu.be/5bWPTTFYsD8](https://youtu.be/5bWPTTFYsD8)

### Four Strategies for Mitigating Amplified Reflection DDoS Attacks

#### 1. Rate limiting

Rate limiting is a general category of DDoS mitigation strategies. The limits can be applied to destinations or to sources. Destination rate limiting is fraught with collateral damage due to its indiscriminating nature and should only be applied as a last course of action to prevent the system from falling over. Rate limiting the source is more effective, as it is done based on a deviation from a set access policy. Restricting these noisy sources or even dropping the UDP fragmented packets from these sources will greatly reduce the impact.

#### 2. Regular Expression (Regex) filter

Applying traffic signature filters can be an effective defense against reflected amplification attacks. These attacks have identifiable repetitive structures from which a regular expression can be derived.\
One drawback of Regex filtering may be performance. DDoS defenses sit at the edge of the networks and must absorb the full volume of a business’s internet capacity. Regardless of whether the inspection is done in software or hardware, inspecting every packet may overwhelm the defenses.

#### 3. Port Blocking

Blocking unneeded ports is always good security practice. The challenge is defending ports that are shared by both legitimate and attacker traffic. DNS’s TCP or UDP port 53 are good examples of required ports that are commonly attacked. Blocking port 53 would have the same effect as a DoS attack on everyone in the environment. On the other hand, blocking port 1900 traffic sourced from the internet makes a lot of sense, since SSDP is an unlikely legitimate use case across the internet.

#### 4. Threat intelligence

Attackers continuously scan the internet looking for servers to employ in their DDoS campaigns. The identity of these vulnerable servers are available to as real-time feeds from threat intelligence companies.
