# the overview of hardware requirement

```mermaid
graph LR
    A[1 Hardware System]

    A --> B1[1.1 Drone]
    B1 --> C11[1.1.1 Drone - CC]

    C11 --> D111[1.1.1.1 CPU/DDR/UFS]
    C11 --> D112[1.1.1.2 Power/Charger]
    C11 --> D113[1.1.1.3 Battery]
    C11 --> D114[1.1.1.4 Long Range]
    C11 --> D115[1.1.1.5 GPS]
    C11 --> D116[1.1.1.6 TPM]
    C11 --> D117[1.1.1.7 Navi Camera]
    C11 --> D118[1.1.1.8 VIO Camera]
    C11 --> D119[1.1.1.9 WiFi]
    C11 --> D1110[1.1.1.10 BT]
    C11 --> D1111[1.1.1.11 5GModem]

    %% Click events (link to GitHub Issues)
    click A "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/21"
    click B1 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/22"
    click C11 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/23"
    click D111 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/24"
    click D112 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/25"
    click D113 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/26"
    click D114 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/27"
    click D115 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/28"
    click D116 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/29"
    click D117 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/30"
    click D118 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/31"
    click D119 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/32"
    click D1110 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/33"
    click D1111 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/34"

    B1 --> C12[1.1.2 Drone - FC]
    C12 --> D121[1.1.2.1 MCU/Flash/RAM]
    C12 --> D122[1.1.2.2 SiK/ELRS]
    C12 --> D123[1.1.2.3 GPS]
    C12 --> D124[1.1.2.4 SE050]
    C12 --> D125[1.1.2.5 IOMCU]

    %% Click events (link to GitHub Issues)
    click C12 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/35"
    click D121 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/36"
    click D122 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/37"
    click D123 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/38"
    click D124 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/39"
    click D125 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/40"

    B1 --> C13[1.1.3 Drone - ESC]
    B1 --> C14[1.1.4 Drone - Spot Light]
    B1 --> C15[1.1.5 Drone - Loud Speaker]
    B1 --> C16[1.1.6 Drone - Night Sense]

    %% Click events (link to GitHub Issues)
    click C13 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/41"
    click C14 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/42"
    click C15 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/43"
    click C16 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/44"

    A --> B2[1.2 RC]
    B2 --> C21[1.2.1 CPU/DDR/UFS]
    B2 --> C22[1.2.2 Power/Charger]
    B2 --> C23[1.2.3 Battery]
    B2 --> C24[1.2.4 Long Range]
    B2 --> C25[1.2.5 SiK/ELRS]
    B2 --> C26[1.2.6 GPS]
    B2 --> C27[1.2.7 WiFi]
    B2 --> C28[1.2.8 BT]
    B2 --> C29[1.2.9 5GModem]
    B2 --> C210[1.2.10 Panel]
    B2 --> C211[1.2.11 Audio]
    B2 --> C212[1.2.12 Joystick]
    B2 --> C213[1.2.13 HDMI]

    %% Click events (link to GitHub Issues)
    click B2 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/45"
    click C21 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/46"
    click C22 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/47"
    click C23 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/48"
    click C24 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/149"
    click C25 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/49"
    click C26 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/50"
    click C27 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/51"
    click C28 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/52"
    click C29 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/53"
    click C210 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/54"
    click C211 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/55"
    click C212 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/56"
    click C213 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/57"

    A --> B3[1.3 Gimbal]
    B3 --> C31[1.3.1 Camera Subsystem]
    C31 --> D131[1.3.1.1 CPU/DDR/UFS]
    C31 --> D132[1.3.1.2 Power/Charger]
    C31 --> D133[1.3.1.3 Battery]
    C31 --> D134[1.3.1.4 Ethernet]
    C31 --> D135[1.3.1.5 USB]
    C31 --> D136[1.3.1.6 Normal Camera]
    C31 --> D137[1.3.1.7 Tele Camera]
    C31 --> D138[1.3.1.8 Wide Camera]

    %% Click events (link to GitHub Issues)
    click B3 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/58"
    click C31 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/59"
    click D131 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/60"
    click D132 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/61"
    click D133 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/62"
    click D134 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/63"
    click D135 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/64"
    click D136 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/65"
    click D137 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/66"
    click D138 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/67"


    B3 --> C32[1.3.2 Motor Subsystem]
    C32 --> D231[1.3.2.1 Support needed from 3rd Vendor]

    %% Click events (link to GitHub Issues)
    click C32 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/68"
    click D231 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/69"
