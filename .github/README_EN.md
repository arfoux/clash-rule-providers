# Clash Rule Providers

Ultimate resource for Clash Rule Providers, offering pre-configured rules that seamlessly integrate with your Clash system for managing network traffic. With our continuously updated rule collection, this repository empowers you to optimize proxy settings and ad blocking efficiently. Ideal for developers and users seeking granular control over their browsing experience.

**Key Features:**

- **Easy Integration:** Directly import configuration files and rules into your Clash system.
- **Regular Updates:** Rules and resource lists are frequently updated for optimal performance and security.
- **Traffic Management:** Simplify proxy and ad-blocking settings with well-structured rules.

## OISD Big (Frequently Used)
**Blocks ads, phishing, malvertising, malware, spyware, ransomware, cryptojacking, scams, and more.**

To use, edit `config.yaml` in your Clash system (usually at the bottom):

```yaml
rule-providers:
  big:
    type: http
    behavior: domain
    url: [https://raw.githubusercontent.com/arfoux/clash-rule-providers/main/big.txt](https://raw.githubusercontent.com/arfoux/clash-rule-providers/main/big.txt)
    path: ./providers/rule-provider_clash.yaml
    interval: 86400
rules:
  - RULE-SET,big,REJECT
```

## OISD Small
**Blocks ads and other annoyances.**

To use, edit `config.yaml` in your Clash system (usually at the bottom):

```yaml
rule-providers:
  small:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/arfoux/clash-rule-providers/main/small.txt
    path: ./providers/rule-provider_clash.yaml
    interval: 86400
rules:
  - RULE-SET,small,REJECT
```

## Kredit
- [OISD Blocklist - oisd.nl](https://oisd.nl/)
