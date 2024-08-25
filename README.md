# Clash Rule Providers
[see English](https://github.com/arfoux/clash-rule-providers/blob/main/.github/README_EN.md)

Pusat sumber daya terlengkap untuk Clash Rule Providers, menyediakan konfigurasi dan aturan yang terintegrasi dengan sistem Clash untuk mengelola trafik jaringan Anda. Dengan koleksi aturan yang selalu diperbarui, repository ini membantu Anda mengoptimalkan pengaturan proxy dan pemblokiran iklan secara efisien. Ideal untuk pengembang dan pengguna yang menginginkan kontrol penuh atas pengalaman browsing mereka.

- **Integrasi Mudah:** Menyediakan file konfigurasi dan aturan yang dapat diimpor langsung ke dalam sistem Clash Anda.
- **Pembaharuan Berkala:** Aturan dan daftar sumber daya diperbarui secara rutin untuk memastikan efektivitas dan keamanan.
- **Pengelolaan Trafik:** Menyederhanakan pengaturan proxy dan pemblokiran iklan dengan aturan yang terstruktur dengan baik.

## OISD Big (Sering dipakai)
**Memblokir Iklan, Phishing, Malvertising, Malware, Spyware, Ransomware, CryptoJacking, Scam, dan lain-lain.**

Untuk menggunakan, edit `config.yaml` pada sistem Clash Anda (biasanya ada di bagian paling bawah):

```yaml
rule-providers:
  big:
    type: http
    behavior: domain
    url: https://raw.githubusercontent.com/arfoux/clash-rule-providers/main/big.txt
    path: ./providers/rule-provider_clash.yaml
    interval: 86400
rules:
  - RULE-SET,big,REJECT
```

## OISD Small
**Memblokir Iklan, dan beberapa hal yang mengganggu**

Untuk menggunakan, edit `config.yaml` pada sistem Clash anda (biasanya ada di bagian paling bawah)

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
