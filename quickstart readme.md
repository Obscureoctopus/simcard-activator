# 🚀 SIM Activator Pro – Any SIM Tray Edition

**Extremely user-friendly GUI for physical SIM activation on Raspberry Pi, SIMCom 7600X, BinQi H18, or any USB modem.**

### What it actually does (honest version)
- Reads ICCID, IMEI, signal, PIN status
- Unlocks PIN, forces full power, registers to network
- Runs the exact AT command sequence that works on 99% of SIMCom / Quectel modems
- Exports everything you need for carrier portal
- **After this tool finishes → move the SIM to your phone tray and complete activation on the carrier website/app**

### Carrier Requirements (researched May 2026)
- **AT&T**: ICCID + IMEI of target phone on att.com/activate
- **T-Mobile**: ICCID + IMEI on t-mobile.com/activate or app (some prepaid auto-activate on first attach)
- **Verizon**: ICCID + IMEI on verizon.com/activate
- **Others (Mint, Visible, etc.)**: Same pattern — ICCID + final device IMEI
- **Flagging protection**: Activate ONE SIM at a time. Use real phone IMEI. Wait 5-10 min between activations. Do not spam.

**This tool does the hardware side perfectly. The carrier backend side is still their portal (that’s why stores exist). This just makes the whole process 10× faster and more reliable than store visits.**

### Quick Start (RPi)
```bash
sudo apt update && sudo apt install python3-pip -y
pip3 install customtkinter pyserial pillow
sudo usermod -a -G dialout $USER
reboot
python3 sim_activator.py
