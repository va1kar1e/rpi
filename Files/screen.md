# Screen

## [Fix] HDMI No Signal

1. Unattach a microsd card and Insert to PC
2. Goto Drive and uncomment this in **config.txt**

    ```plaintext
    # uncomment if you get no picture on HDMI for a default "safe" mode
    hdmi_safe=1
    
    ...
    
    # uncomment if hdmi display is not detected and composite is being output
    hdmi_force_hotplug=1
    ```

## [MHS-3.5inch RPi Display Screen](mhs-3.5.md)
