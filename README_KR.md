
DBOT Project (개발중)  
이 프로젝트는 개인 프로젝트 입니다.  
  
Lostroid는 사람의 잃어 버린 조각을 채워 주는 로봇을 생각 해서 만들지는 않고    
다음과 같은 이유로 만들게 되었습니다.  
- 우선 아무도 안사용 하는 이름 선정 (구글 기타 계정에 사용 안하는 이름 사용)  
- 안드로이드 이름을 포함 시키고 싶었음.  
이런 이유로 이름을 정하였습니다.  
  
이 프로젝트의 최종 목표는 IOT 홈 네트워크 관리 비서 + 홈끼리 그룹 + 약간의 AI 흉내를 목표로 합니다.  
  
혼자서 개발 할때 해야 될 일  
아래 순서대로 하는게 아니고 동시 다발 적으로 진행 하며
부품과 수급 에따라 내용을 변경 바로바로 수정할 수 있게 진행 합니다.

1. 사양 (기능) 결정  
   1.1. WIFI, Bluetooth, Zigbee, 유선 100Mbps 를 제공  
   1.2. SPI TFT LCD 듀얼 모니터 제공 (메뉴및 정보 화면, AI화면)  
   1.3. camera 사물 인식  
   1.4. 음성 인식에 필요 한 MIC  
   1.5. 동작을 제어할 모터  
   1.6. 소리를 내보낼 스피커  
   1.7. 보조 배터리 내장  
   1.8. 사용자 버튼  
   1.9. MAIN MCU + 배터리 MCU 2개의 구조로 결정  
     
2. 부품선정  
   부품선정은 다음과 같은 기준으로 선정 했습니다.  
   - 부품 구매가 쉬워야 한다.  
   - 가격이 저렴해야 된다.  
   
   2.1. MCU  
     Main MCU: STM32H5  
     Battery MCU: STM32C071G8U6  
    
   2.2. 배터리  
     보호회로가 있는 CELL  
     고방전 5000mA 15A 21700  
  
   2.3. 스피커  
     풀레인지 40mm  

   2.4. 디스플레이  
    - 2.4 or 2.8 Inch 320x240 SPI  
    - 1.8 Inch  180x160 SPI  
     
   2.5. 카메라  
    - OV2640, OV5640  
  
   2.6.  

3. 디자인  
   3.1 기본적으로 큐브 형태의 모형을 스케지 부품의 배치만 그림
     
   <p align = "center"><img width="674" height="1256" alt="Image" src="https://github.com/user-attachments/assets/59d6dc75-5dd9-406d-bb39-c6bac430ac92" /></p>

   3.2 실제 기구 구현 개발중
    <p align = "center"><img width="720" height="654" alt="Image" src="https://github.com/user-attachments/assets/513b79fa-1c4b-4784-b7d9-245ca5d8ef57" /></p>  
    <p align = "center"><img width="720" height="641" alt="Image" src="https://github.com/user-attachments/assets/a44884a2-bf39-448d-9962-67ac35c033e4" /></p>  
    <p align = "center"><img width="720" height="937" alt="Image" src="https://github.com/user-attachments/assets/9af78e70-7521-4753-81ed-ec594454c53d" /></p>  

5. PCB 만들기
   4.1 Battery PCB
<p align = "center"><img width="720" height="498" alt="Image" src="https://github.com/user-attachments/assets/c65f6b3d-515f-4cbf-b071-9020154c6f7f" /></p>
<p align = "center"><img width="720" height="496" alt="Image" src="https://github.com/user-attachments/assets/d1264ea0-20f2-4a0b-892b-0fb45ecb530e" /></p>
<p align = "center"><img width="800" height="704" alt="Image" src="https://github.com/user-attachments/assets/34eb4267-0a4c-4826-a956-71eae0bdb80f" /></p>
<p align = "center"><img width="800" height="704" alt="Image" src="https://github.com/user-attachments/assets/44e1c0db-af4b-4281-bb4f-ea33f568e458" /></p>
<p align = "center"><img width="800" height="737" alt="Image" src="https://github.com/user-attachments/assets/450d9217-da8e-418c-abff-0c26f0ded5fe" /></p>
<p align = "center"><img width="800" height="685" alt="Image" src="https://github.com/user-attachments/assets/9058a5f1-2d0d-4df4-aeb4-0bcd62ccbd83" /></p>

