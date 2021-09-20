# Wifi Network

- Scan interface Wlan0 and add Nework at **wpa_supplicant.conf**

    ```bash
    sudo iwlist wlan0 scan
    sudo vim /etc/wpa_supplicant/wpa_supplicant.conf
    ```

    **add**

    ```
    country=TH
    ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
    update_config=1

    network={
    	ssid="valkarie_2"
    	psk="pqh47m9nr4"
    }

    network={
    	ssid="Valkaries_share"
    	psk="aryd9306"
    }

    network={
    	ssid="sugus"
    	psk="R0ll0ut!"
    }
    ```

    or follow gui with this command

    ```bash
    sudo raspi-config
    ```

- Check Wlan0 interface

    ```bash
    ifconfig wlan0
    ```

!!! **Fix Problem** Interface can not communicate with `wpa_supplicant`

```bash
sudo killall wpa_supplicant
sudo wpa_supplicant -c/etc/wpa_supplicant/wpa_supplicant.conf -iwlan0
```
