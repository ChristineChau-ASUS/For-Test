# Software Requirements Overview

Author / Maintainer: ChristineChau-ASUS &nbsp; | &nbsp; Last Updated: 2026/04/30

```mermaid
graph LR
    A2["2 Software System"]

    %% 2.1
    A2 --> B21["2.1 Device Activation & Verification"]

    B21 --> C211["2.1.1 CC"]
    C211 --> D2111["2.1.1.1 Secure Boot and TrustZone support"]
    C211 --> D2112["2.1.1.2 Define all required keys (CC/FC/GB)"]
    C211 --> D2113["2.1.1.3 Secure key storage"]

    B21 --> C212["2.1.2 FC"]
    C212 --> D2121["2.1.2.1 Secure Boot support"]
    C212 --> D2122["2.1.2.2 Secure key storage"]

    B21 --> C213["2.1.3 GB"]
    C213 --> D2131["2.1.3.1 Secure Boot and TrustZone support"]
    C213 --> D2132["2.1.3.2 Secure key storage"]

    B21 --> C214["2.1.4 CC Diagnosis"]
    C214 --> D2141["2.1.4.1 Detect and correct hardware deviations"]
    C214 --> D2142["2.1.4.2 LED status indication (ready)"]

    B21 --> C215["2.1.5 FC Diagnosis"]
    C215 --> D2151["2.1.5.1 Detect and correct hardware deviations"]
    C215 --> D2152["2.1.5.2 LED status indication (ready)"]

    B21 --> C216["2.1.6 GB Diagnosis"]
    C216 --> D2161["2.1.6.1 Detect and correct hardware deviations"]
    C216 --> D2162["2.1.6.2 LED status indication (ready)"]

    B21 --> C217["2.1.7 Network Bootstrap"]
    C217 --> D2171["2.1.7.1 Internet access method"]
    C217 --> D2172["2.1.7.2 Wi-Fi hotspot + BLE provisioning"]
    C217 --> D2173["2.1.7.3 BLE/GATT profile & message format"]

    B21 --> C218["2.1.8 Secure Onboarding"]
    C218 --> D2181["2.1.8.1 FDO secure onboarding"]
    C218 --> D2182["2.1.8.2 Lighthouse registration (overlay IP)"]

    B21 --> C219["2.1.9 Call Home Process"]
    C219 --> D2191["2.1.9.1 Call Home agent"]

    B21 --> C2110["2.1.10 Firmware Update (FOTA)"]
    C2110 --> D21101["2.1.10.1 IoT Server"]
    C2110 --> D21102["2.1.10.2 MP Server"]

    %% 2.2
    A2 --> B22["2.2 Swarm Management"]
    B22 --> C221["2.2.1 Web UI"]
    B22 --> C222["2.2.2 Swarm inspection selection"]
    B22 --> C223["2.2.3 Team & configuration setup"]
    B22 --> C224["2.2.4 Default swarm setup"]

    %% 2.3
    A2 --> B23["2.3 Mission Task Management"]
    B23 --> C231["2.3.1 Define mission parameters"]
    B23 --> C232["2.3.2 Restricted zone map data"]
    B23 --> C233["2.3.3 Preflight Go/No-Go gate expansion"]
    B23 --> C234["2.3.4 Default mission task"]

    %% 2.4
    A2 --> B24["2.4 Flight Mission Execution"]
    B24 --> C241["2.4.1 Failsafe functions"]
    B24 --> C242["2.4.2 Single-drone monitoring"]
    B24 --> C243["2.4.3 Swarm overview"]
    B24 --> C244["2.4.4 Gimbal control"]
    B24 --> C245["2.4.5 Camera control"]

    %% 2.5
    A2 --> B25["2.5 Drone RC Interface API"]
    B25 --> C251["2.5.1 MAVLink v2 commands"]
    B25 --> C252["2.5.2 YANG schema"]
    B25 --> C253["2.5.3 Additional APIs"]

    %% Click mapping (only for defined nodes)
    click A2 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/70"
    click B21 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/71"
    click C211 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/72"

    click D2111 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/73"
    click D2112 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/74"
    click D2113 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/75"

    click C212 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/76"
    click D2121 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/77"
    click D2122 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/78"

    click C213 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/79"
    click D2131 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/80"
    click D2132 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/81"

    click C214 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/82"
    click D2141 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/83"
    click D2142 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/84"

    click C215 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/85"
    click D2151 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/86"
    click D2152 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/87"

    click C216 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/88"
    click D2161 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/89"
    click D2162 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/90"

    click C217 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/91"
    click D2171 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/92"
    click D2172 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/93"
    click D2173 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/94"

    click C218 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/95"
    click D2181 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/96"
    click D2182 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/97"

    click C219 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/98"
    click D2191 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/99"

    click C2110 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/100"
    click D21101 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/101"
    click D21102 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/102"

    click B22 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/103"
    click C221 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/104"
    click C222 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/105"
    click C223 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/106"
    click C224 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/107"

    click B23 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/108"
    click C231 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/109"
    click C232 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/110"
    click C233 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/111"
    click C234 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/112"

    click B24 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/113"
    click C241 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/150"
    click C242 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/114"
    click C243 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/115"
    click C244 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/116"
    click C245 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/117"

    click B25 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/118"
    click C251 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/119"
    click C252 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/120"
    click C253 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/121"

    click B26 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/151"
    click C261 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/152"
    click C262 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/153"
    click C263 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/154"

    click B27 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/122"
    click C271 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/123"
    click C272 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/124"
    click C273 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/125"
    click C274 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/126"
    click C275 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/127"

    click B28 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/128"
    click C281 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/129"

    click D2811 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/130"
    click D2812 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/131"
    click D2813 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/132"

    click C282 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/133"
    click D2821 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/134"
    click D2822 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/135"

    click C283 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/136"
    click D2831 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/137"

    click C284 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/138"
    click D2841 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/139"

    click C285 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/155"

    click D2851 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/156"
    click D2852 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/157"
    click D2853 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/140"
    click D2854 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/158"
    click D2855 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/141"

    click C286 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/142"

    click D2861 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/143"
    click D2862 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/144"
    click D2863 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/145"
    click D2864 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/146"
    click D2865 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/147"
    click D2866 "https://github.com/Asus-Robotics-and-AI-Center/requirements/issues/148"
