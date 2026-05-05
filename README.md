# simcard-activator v2  
# 🚀 SIM Activator Pro v2 – Swiss Army Knife for Physical SIM Cards

**Everything you can do to a physical SIM card – in one buttery-smooth GUI.**

Works perfectly on:
- Raspberry Pi + SIMCom 7600X-B HAT
- BinQi H18 PTT radio
- Any USB modem with SIM tray (SIMCom, Quectel, Huawei, etc.)

**Features (literally every AT command you’ll ever need):**
- Activation Wizard
- Diagnostics Dashboard
- Full SMS Manager
- USSD Dialer
- Advanced SIM File Access
- Bulk Activation
- Raw AT Terminal + 100+ command presets

**Quick start on RPi:**
```bash
sudo apt update && sudo apt install python3-pip -y
pip3 install customtkinter pyserial pillow pandas
sudo usermod -a -G dialout $USER && reboot
python3 sim_activator_v2.py
