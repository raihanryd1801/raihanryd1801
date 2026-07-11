```
┌────────────────────────────────────────────────────────────────────┐
│                                                                    │
│   ██████╗  █████╗ ██╗██╗  ██╗ █████╗ ███╗   ██╗                 │
│   ██╔══██╗██╔══██╗██║██║  ██║██╔══██╗████╗  ██║                 │
│   ██████╔╝███████║██║███████║███████║██╔██╗ ██║                 │
│   ██╔══██╗██╔══██║██║██╔══██║██╔══██║██║╚██╗██║                 │
│   ██║  ██║██║  ██║██║██║  ██║██║  ██║██║ ╚████║                 │
│   ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═══╝                 │
│                                                                    │
│                    ██╗███╗   ██╗███████╗██████╗  █████╗           │
│                    ██║████╗  ██║██╔════╝██╔══██╗██╔══██╗          │
│                    ██║██╔██╗ ██║█████╗  ██████╔╝███████║          │
│                    ██║██║╚██╗██║██╔══╝  ██╔══██╗██╔══██║          │
│                    ██║██║ ╚████║██║     ██║  ██║██║  ██║          │
│                    ╚═╝╚═╝  ╚═══╝╚═╝     ╚═╝  ╚═╝╚═╝  ╚═╝          │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

```
╔═══════════════════════════════════════════════════════════════════════════════╗
║  [SYSTEM]  : 0x52414948414E                                                  ║
║  [NODE]    : raihanryd1801                                                   ║
║  [UPTIME]  : 42d 7h 23m 11s                                                  ║
║  [ROLE]    : NOC ENGINEER | NETWORK ARCHITECT | VOIP SPECIALIST              ║
║  [STATUS]  : 🔴 LIVE - DO NOT INTERRUPT                                      ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

---

## 🖥️ ACTIVE SESSIONS

```
$> who
raihan   pts/0        2024-01-15 08:42 (10.0.0.100)
raihan   pts/1        2024-01-15 09:13 (10.0.0.101)
raihan   pts/2        2024-01-15 09:45 (10.0.0.102)
```

```
$> lastlog | grep -v "Never logged in"
Username     Port     From             Latest
raihan       pts/0    10.0.0.100       Mon Jan 15 08:42:23 +0700 2024
root         pts/0    192.168.1.1      Mon Jan 15 07:15:02 +0700 2024
```

---

## 🌐 NETWORK TOPOLOGY

```
                      ┌─────────────┐
                      │  INTERNET   │
                      └──────┬──────┘
                             │
                      ┌──────▼──────┐
                      │  FIREWALL   │
                      │   (pfSense) │
                      └──────┬──────┘
                             │
                ┌────────────┼────────────┐
                │            │            │
         ┌──────▼─────┐ ┌───▼────┐ ┌─────▼─────┐
         │  SWITCH-01 │ │SWITCH-02│ │  SWITCH-03│
         │  (Cisco)   │ │(MikroTik)│ │  (HP)    │
         └──────┬─────┘ └───┬────┘ └─────┬─────┘
                │           │            │
      ┌─────────┼───────────┼────────────┼─────────┐
      │         │           │            │         │
   ┌──▼──┐  ┌───▼──┐   ┌────▼───┐  ┌────▼───┐ ┌──▼──┐
   │VOIP │  │SERVERS│   │CLIENTS │  │PRINTERS│ │APs  │
   │GW   │  │(Proxmox)│ │(DHCP)  │  │(Network)│ │(WiFi)│
   └─────┘  └───────┘   └────────┘  └────────┘ └─────┘
```

---

## 📊 LIVE METRICS

```
$> htop --real-time
```

![Raihan's GitHub Stats](https://github-readme-stats.vercel.app/api?username=raihanryd1801&show_icons=true&theme=radical&hide_border=true&bg_color=0D1117&title_color=00FF41&icon_color=00FF41&text_color=00FF41)

```
┌─────────────────────────────────────────────────────┐
│ CPU:  ████████████░░░░░░░░░░  42.3%                │
│ RAM:  ████████████████░░░░░░  68.7%                │
│ DISK: ██████████████████████  92.1%                │
│ NET:  ████████░░░░░░░░░░░░░░  31.5%                │
│ VOIP: ██████████████████████  100% JITTER FREE     │
└─────────────────────────────────────────────────────┘
```

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=raihanryd1801&layout=compact&theme=radical&hide_border=true&bg_color=0D1117&title_color=00FF41&text_color=00FF41)

---

## 🛠️ INFRASTRUCTURE STACK

```bash
$> netstat -tulpn | grep LISTEN
```

```
PORT     SERVICE     VERSION          STATUS
22       SSH         OpenSSH 9.5      🔒 SECURE
80       HTTP        Nginx 1.24.0     🌐 ONLINE
443      HTTPS       SSL/TLS 1.3      🔐 ENCRYPTED
5060     SIP         Asterisk 18      📞 VOIP ACTIVE
5061     SIPS        Asterisk 18      📞 SECURE VOIP
3306     MySQL       8.1.0            🗄️ ONLINE
6379     Redis       7.2.0            ⚡ CACHE
8080     HTTP        Docker/Proxy     🐳 CONTAINER
```

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  LANGUAGES    │ PHP ■■■■■■■■■■ 78%                  
               │ JS  ■■■■■■■■■■ 65%                  
               │ SQL ■■■■■■■■■■ 55%                  
               │ Python■■■■■■ 30%                     
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  FRAMEWORKS   │ Laravel    ■■■■■■■■■■■ 90%          
               │ Bootstrap  ■■■■■■■■■■ 80%           
               │ Tailwind   ■■■■■■■■■■ 75%           
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  DATABASES    │ MySQL      ■■■■■■■■■■■ 95%          
               │ MariaDB    ■■■■■■■■■■ 80%           
               │ Redis      ■■■■■■■■ 60%             
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
  VIRTUAL      │ Proxmox    ■■■■■■■■■■■ 95%          
               │ Docker     ■■■■■■■■■■■ 90%           
               │ LXC        ■■■■■■■■■■ 75%           
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

---

## 🔐 SECURITY LOG

```
$> tail -f /var/log/auth.log
```

```
[Jan 15 09:45:23] SSH: Accepted password for root from 192.168.1.100 port 52341
[Jan 15 09:46:12] SIP: Registration successful - extension 1001@voip.local
[Jan 15 09:47:05] FIREWALL: Blocked port scan from 45.33.22.11 (DROP)
[Jan 15 09:48:30] VPN: Tunnel established - 10.8.0.2 (site-to-site)
[Jan 15 09:49:15] NETWORK: BGP neighbor 10.0.0.1 established (AS 65001)
[Jan 15 09:50:02] VOIP: Call initiated - 1001 -> 1002 (RTP stream active)
```

---

## ⚡ ACTIVE PROJECTS

```
┌────────────────────────────────────────────────────────────────────┐
│ PROJECT: Network Automation Suite                                 │
│ STATUS : 🚧 UNDER DEVELOPMENT                                    │
│ STACK  : Python + Ansible + Netmiko                             │
│ TARGET : 50+ Network Devices                                     │
├────────────────────────────────────────────────────────────────────┤
│ PROJECT: VoIP Monitoring Dashboard                                │
│ STATUS : 🔴 LIVE PRODUCTION                                     │
│ STACK  : Laravel + WebRTC + FreeSwitch                          │
│ TARGET : 1000+ Concurrent Calls                                  │
├────────────────────────────────────────────────────────────────────┤
│ PROJECT: Infrastructure as Code                                   │
│ STATUS : 🟢 DEPLOYED                                            │
│ STACK  : Terraform + Docker + Proxmox                           │
│ TARGET : 100% Automation                                         │
└────────────────────────────────────────────────────────────────────┘
```

---

## 📡 CONNECT WITH ME

```
$> dig +short A raihan.local
```

```yaml
ENCRYPTED_CHANNEL:
  linkedin: https://linkedin.com/in/raihanryd/
  email:    raihan.ryd@dankom.co.id
  github:   https://github.com/raihanryd1801
  pgp_key:  0x52414948414E
  
  response_time: < 24 hours
  encryption:    AES-256-GCM
  signature:     Verified
```

---

## 🎯 MISSION STATEMENT

```javascript
const mission = () => {
  while (network.running) {
    optimizeBandwidth();
    secureEndpoints();
    automateDeployments();
    monitorVOIPQuality();
    documentEverything();
  }
};

setInterval(mission, 1000);
```

---

```
╔═══════════════════════════════════════════════════════════════════════════════╗
║                                                                            ║
║  ╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗╔═══╗               ║
║  ║███║║███║║███║║███║║███║║███║║███║║███║║███║║███║║███║               ║
║  ╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝╚═══╝               ║
║                                                                            ║
║  [SYSLOG] SESSION TERMINATED - NODE OFFLINE                                ║
║  [PID]    : 1801                                                           ║
║  [UPTIME] : 42d 7h 23m 11s                                                ║
║  [QUOTE]  : "In God we trust, all others must bring network diagrams"      ║
║                                                                            ║
╚═══════════════════════════════════════════════════════════════════════════════╝
```

---

*Maintained with ☕, 🍜, and unlimited bandwidth by [raihanryd1801](https://github.com/raihanryd1801)*

```
PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data.
64 bytes from 8.8.8.8: icmp_seq=1 ttl=117 time=12.3 ms
--- Connection Stable ---
```

**⚠️ This node is optimized for dark mode. Enable it for maximum stealth.** 🕶️
