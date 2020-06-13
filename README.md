# Realtek 8811CU driver for Raspbian

Driver for 802.11ac USB adapter with RTL8811CU or RTL8821CU chipset, only STA/Monitor mode is supported, no AP mode.

Currently tested with Linux kernel 4.19.97-v7+ on Raspberry Pi 3 B+.

### Manual installation

To build, you have to retrieve source and run `make`.
If via Git, do following:

```bash
sudo apt-get install raspberrypi-kernel-headers
git clone https://github.com/fastoe/RTL8811CU_for_Raspbian
cd RTL8811CU_for_Raspbian
make -j4 && sudo make install
sudo modprobe 8821cu
sudo reboot
```

Enjoy!
