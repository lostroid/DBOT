
# 2025년도 개인 프로젝트 DBOT (중단)
### 중단 이유
1. 너무 무거움 기구 설계의 복잡 스피커가 너무 큼.
2. 배터리 제어 부와 상단 제어 부 생각보다 많은 작업이 필요 장시간 걸림.

### 다시 시작 예정
1. 큐빅모양 경량
2. 데스크탑 특성상 이동 위험을 고려 고정형
3. 팔이나 머리 만 움직이는 형태 사용자를 인식 수준

<p align="center">
<img width="600" height="815" alt="image" src="https://github.com/user-attachments/assets/2e5991ed-9644-46e7-8182-533d2de4a931" />
<img width="600" height="616" alt="image" src="https://github.com/user-attachments/assets/7722a9d8-ee05-48d3-8c40-568318ee257d" />
</p>
  
## 목표  
### 목적  
* 책상 위에 고정된 로봇 공부  
* 일반 DC 모터 및 BLDC 혼합 동작 공부  
* 배터리 충전 IC 공부  
* 전류, 전압 모니터링 공부  
* 디스플레이 공부  
* 터치 스크린 공부  
* 유선 Ethernet 공부  
* WIFI, BLUETOOTH, Zigbee  통신 공부  
* 카메라 공부
* MicroSD Card 공부
* 스피커 앰프 공부
  
### 활용 Interface  
* I2C : 온도 습도
* UART : 디버깅
* SPI : 디스플레이
* DCMI : 카메라 (OV2640 또는 OV5640)
* SDIO : MicroSD (FAT32) 파일시스템
* RMII : 100MBPS PHY
* SAI : 스피커 앰프 통신
* ADC : 전류, 전압 모니터링

### 부품 선정
1 MCU  
  Main 보드 : STM32H553  
  Battery 보드: STM32C071G8U6  
  
2 Battery  
  5000 mA  PCM 내장


  
<img width="957" height="712" alt="image" src="https://github.com/user-attachments/assets/e3ec6b2c-e0b1-474c-835b-3c009261b1d9" />

I'm not good at English, so I used a translation.    
  
DBOT Project (B01)  
This is a personal project.  
  
Lostroid was not created with the idea of a robot that fills in the missing pieces of a person.  
It was created for the following reasons:  
  First, to choose a name that no one else is using (a name not used on Google or other accounts).  
  I wanted to include “Android” in the name.  
  For these reasons, the name was decided.  
  
Final Goal of This Project  
The ultimate goal of this project is to create:  
An IoT home network management assistant + grouping between homes + a bit of AI imitation.  
  
Tasks to Do When Developing Alone  
  
1. Specification (Function) Definition  
  1.1. Provide: WiFi, Bluetooth, Zigbee, Wired 100Mbps  
  1.2. Dual SPI TFT LCD displays (Menu & Information screen, AI screen)  
  1.3. Camera for object recognition  
  1.4. Microphone for voice recognition  
  1.5. Motors to control movement  
  1.6. Speaker for audio output  
  1.7. Built-in auxiliary battery  
  1.8. User buttons  
  1.9. Dual MCU structure: MAIN MCU + Battery MCU  
  
2. Component Selection  
  Components were selected based on the following criteria:  
  Easy to purchase.  
  Low cost.  
  
  2.1 MCU  
    Main MCU: STM32H5  
    Battery MCU: STM32C071G8U6  
  
  2.2 Battery  
    Cell with protection circuit  
    High-discharge 5000mA 15A 21700  
  
  2.3 Speaker  
    40mm full-range speaker  
  
  2.4 Display  
    2.4 or 2.8 inch 320x240 SPI  
    1.8 inch 180x160 SPI  
  
  2.5 Camera  
    OV2640, OV5640  
  
3. Design  
  3.1 Basic Concept  
    Initially sketched in a cube form, focusing only on component placement.  
  <p align = "center"><img width="674" height="1256" alt="Image" src="https://github.com/user-attachments/assets/59d6dc75-5dd9-406d-bb39-c6bac430ac92" /></p>  
  
  3.2 Mechanical Implementation (In Development)  
  <p align = "center"><img width="720" height="654" alt="Image" src="https://github.com/user-attachments/assets/513b79fa-1c4b-4784-b7d9-245ca5d8ef57" /></p>   
  <p align = "center"><img width="720" height="641" alt="Image" src="https://github.com/user-attachments/assets/a44884a2-bf39-448d-9962-67ac35c033e4" /></p>  
  <p align = "center"><img width="720" height="937" alt="Image" src="https://github.com/user-attachments/assets/9af78e70-7521-4753-81ed-ec594454c53d" /></p> 
  
4. PCB Development  
  4.1 Battery PCB  
<p align = "center"><img width="720" height="498" alt="Image" src="https://github.com/user-attachments/assets/c65f6b3d-515f-4cbf-b071-9020154c6f7f" /></p>
<p align = "center"><img width="720" height="496" alt="Image" src="https://github.com/user-attachments/assets/d1264ea0-20f2-4a0b-892b-0fb45ecb530e" /></p>
<p align = "center"><img width="800" height="704" alt="Image" src="https://github.com/user-attachments/assets/34eb4267-0a4c-4826-a956-71eae0bdb80f" /></p>
<p align = "center"><img width="800" height="704" alt="Image" src="https://github.com/user-attachments/assets/44e1c0db-af4b-4281-bb4f-ea33f568e458" /></p>
<p align = "center"><img width="800" height="737" alt="Image" src="https://github.com/user-attachments/assets/450d9217-da8e-418c-abff-0c26f0ded5fe" /></p>
<p align = "center"><img width="800" height="685" alt="Image" src="https://github.com/user-attachments/assets/9058a5f1-2d0d-4df4-aeb4-0bcd62ccbd83" /></p>
  
   
