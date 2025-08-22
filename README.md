# 🍯 Real T-Pot Honeypot IOCs

## ⚠️ REAL ATTACKERS - LIVE HONEYPOT DATA

These IPs **actually attacked** our live T-Pot honeypot infrastructure.

### 📊 Attack Statistics (2025-08-22)
- **Real Attackers**: 8
- **Total Attacks**: 1,900
- **Critical Threats**: 4 (≥200 attacks)
- **High Risk**: 4 (≥100 attacks)
- **Medium Risk**: 0 (≥50 attacks)
- **Data Source**: Live T-Pot Elasticsearch + System Logs

### 🚨 Most Dangerous Attackers (Critical)
- `2.57.121.148` - CRITICAL THREAT
- `45.234.176.18` - CRITICAL THREAT
- `177.43.78.218` - CRITICAL THREAT
- `170.64.198.43` - CRITICAL THREAT

### ⚠️ High Risk Attackers
- `176.88.29.133` - HIGH RISK
- `83.220.35.3` - HIGH RISK
- `113.199.236.53` - HIGH RISK
- `77.79.170.241` - HIGH RISK

### 🔧 Quick Usage
```bash
# Download latest IOCs
curl -s https://raw.githubusercontent.com/xTr1ckst3r/HoneyPot-IOCs/main/daily-iocs/2025-08-22.txt > honeypot-attackers.txt

# Block with iptables (Linux)
while read ip; do 
  iptables -A INPUT -s $ip -j DROP
done < honeypot-attackers.txt

# Block with pfSense/OPNsense
# Import the CSV file for bulk blocking with attack counts
```

### 📈 Data Collection
- **Real-time**: Direct access to T-Pot Elasticsearch
- **Comprehensive**: System logs, Docker logs, network connections
- **Verified**: Only public IPs that actually attempted attacks
- **Fresh**: Updated automatically with live honeypot data

### 📁 Available Files
- `daily-iocs/2025-08-22.txt` - Simple IP list (one per line)
- `daily-iocs/2025-08-22.csv` - Detailed CSV with attack counts
- `daily-iocs/2025-08-22.json` - Complete JSON with metadata

---
🛡️ **Stay Protected** | 🔄 **Real Data** | 🍯 **Live Honeypot**  
*Last updated: 2025-08-22T04:25:41.131112*