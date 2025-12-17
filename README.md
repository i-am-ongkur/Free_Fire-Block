# Free Fire Block

Block the **Free Fire** game from your home network using **AdGuard Home**.

This repository contains a blocklist (DNS rules) that will prevent devices on your network from reaching Free Fire game servers and related domains when applied in AdGuard Home.

---

## 🚀 What This Does

AdGuard Home uses DNS filtering to block domains. This blocklist contains hostnames/domains used by the Free Fire game. When you add this list to AdGuard Home, DNS queries for these domains will be blocked — effectively stopping the game from connecting to its servers. :contentReference[oaicite:1]{index=1}

> ⚠️ This only blocks *network access* to Free Fire. This may not prevent local launch if the game is cached or if alternate DNS/connection methods are used.

---

## 📁 Files

- **BLOCKER.txt** — The blocklist you add to AdGuard Home (domains/rules).
- **README.md** — This documentation.

---

## 📦 How to Install

1. Open your **AdGuard Home dashboard**.
2. Go to **Filters → DNS Blocklists**.
3. Click **Add Custom Blocklist**.
4. Enter the *raw GitHub URL* of `BLOCKER.txt`, for example: https://raw.githubusercontent.com/i-am-ongkur/Free_Fire-Block/main/BLOCKER.txt
   
5. Save and **Apply** the changes.
6. DNS queries for blocked domains should now be dropped.

---

## 🛠 How It Works

AdGuard Home uses filter lists similar to ad blockers. This blocklist is in DNS/domains format — it tells the DNS server to refuse or block requests to Free Fire-related hosts. :contentReference[oaicite:2]{index=2}

You can update the list if new domains need blocking.

---

## 📌 Notes

- If Free Fire still works, the game may be using:
  - **Alternate domains**
  - **Hardcoded IPs**
  - **Encrypted DNS (DoT/DoH)**
  - **VPN bypass**
- For stronger blocking you may need to combine:
  - DHCP + DNS filters
  - Firewall rules
  - Client-based blocks

---

## 📜 License

This project is provided “as-is”. You can use or modify this list personally. There is **no warranty** that it will always work or block every connection.

---

## ❓ Support

If you find any Free Fire domains not blocked, feel free to open an issue or create a pull request with the new domain entries.



