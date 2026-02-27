## Encrypted Live Video Traffic Trace Dataset (PCAP)

Privacy-preserving trace data of encrypted livestream sessions self-collected across multiple platforms, released to support reproducible research on **identification and classification of encrypted livestream traffic**.

## Notes
- Each session lasts **60 seconds** and is saved as a single **PCAP** file.

---

## What’s inside

### Platforms
- **Bilibili**
- **Douyin**
- **Douyu**
- **Huya**

### Transport (in our captures)
- **Bilibili**: observed **both** (i) **HTTPS over TCP** with **TLS 1.2 / TLS 1.3**, and (ii) **QUIC over UDP (HTTP/3)** in some sessions
- **Douyin / Douyu / Huya**: encrypted transport observed in our captures (mainly **TLS over TCP** and/or **QUIC over UDP**, depending on client/network conditions)

### Capture setting
- Controlled **100 Mbps** access rate
- Focus on the **first 60 seconds after the livestream starts**

---
## Raw dataset (PCAP) download
This repository includes our collected platform livestream traffic dataset, UJN-LiveVideo2025 (total 1.1TB).
The download link for the raw PCAP files is: https://pan.baidu.com/s/18AfQYyP78k5IqnnSmyZcHQ?pwd=k8sj

## Contact
If you have questions, please contact: wanghaonan5633@163.com

## Repository structure

```text
├── DataSet/
│   ├── BiliBili/
│   │   ├── game/
│   │   │   └── original/
│   │   ├── chat/
│   │   │   └── original/
│   │   └── entertainment/
│   │       └── original/
│   ├── Douyin/
│   │   ├── game/
│   │   │   └── original/
│   │   ├── chat/
│   │   │   └── original/
│   │   └── entertainment/
│   │       └── original/
│   ├── Douyu/
│   │   ├── game/
│   │   │   └── original/
│   │   ├── chat/
│   │   │   └── original/
│   │   └── entertainment/
│   │       └── original/
│   └── Huya/
│       ├── game/
│       │   └── original/
│       ├── chat/
│       │   └── original/
│       └── entertainment/
│           └── original/
└── README.md


