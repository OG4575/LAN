# LAN síť – Cisco Packet Tracer

## 📡 Popis sítě
Tato LAN síť byla vytvořena v Cisco Packet Traceru a obsahuje:

- 2 switche (S1, S2)
- 2 počítače (PC1, PC2)
- 2 servery:
  - SRV1 (DHCP + DNS)
  - SRV2 (WEB server)

### Topologie:
- PC1 a PC2 jsou připojeny do S1
- S1 je propojen se S2
- SRV1 a SRV2 jsou připojeny do S2

---

## 🌐 IP adresace

| Zařízení | IP adresa | Poznámka |
|----------|----------|----------|
| SRV1     | 192.168.1.1 | DHCP + DNS |
| SRV2     | 192.168.1.2 | Web server |
| PC1      | 192.168.1.10 | Statická IP |
| PC2      | DHCP | Automaticky přidělená IP |

---

## 📡 DHCP nastavení (SRV1)

- DHCP: Zapnuto
- Pool Name: LAN
- Default Gateway: 192.168.1.1
- DNS Server: 192.168.1.1
- Start IP Address: 192.168.1.100
- Subnet Mask: 255.255.255.0

---

## 🌍 DNS nastavení (SRV1)

- DNS: Zapnuto
- Doména:
  - `gola.cz - 192.168.1.2`

---

## 🌐 WEB server (SRV2)

- HTTP: Zapnuto
- Webová stránka (`index.html`):

```html
<h1>Ondřej Gola</h1>
