# 🍪 MOMS Cookie : 아침이 두려운 당신을 위해, 엄마처럼 챙겨주는 스마트 알람 비서

<div align="center">
  <p>더이상의 "5분만 더"는 없다</p>
</div>

---

## 🧠 프로젝트 소개

**MOM's Cookie는** 센서, AI, Wi-Fi 연동 기능을 갖춘 스마트 알람 시스템으로, 바쁜 현대인의 아침을 자동화해주는 IoT 기반의 AI 비서 프로젝트입니다.
하드웨어와 소프트웨어를 통합하여, 사용자의 아침 루틴을 자동화하고 최적화합니다.

---

## 💡 주요 기능

- **AI 비서 기능**  
  사용자의 음성을 인식해 GPT-4 Turbo를 통해 아침 인사, 일정 요약, 날씨 정보 등을 제공합니다.

- **센서 기반 자동 알람**  
  온습도, 빛 감지 등을 바탕으로 알람 조건을 자동 설정하고, 상황에 따라 맞춤형 반응을 합니다.

- **일정 관리 연동**  
  Google Calendar와 연동해 당일 일정을 음성으로 안내합니다.

- **하드웨어 제어**  
  STM32, Arduino Mega, ESP8266 등의 보드를 통해 센서 및 출력 장치를 제어합니다.

- **Wi-Fi 통신 모듈**  
  ESP32를 통해 서버와 통신하여 API로 데이터를 주고받고, 비서 기능과 일정 기능을 연결합니다.

---

##  🛠️ 사용 기술들

✅ 프로그래밍 언어

<img src="https://img.shields.io/badge/c++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white"> <img src="https://img.shields.io/badge/c-A8B9CC?style=for-the-badge&logo=c&logoColor=white"> <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">

✅ 임베디드 & 하드웨어

<img src="https://img.shields.io/badge/arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white"> <img src="https://img.shields.io/badge/stm32-03234B?style=for-the-badge&logo=stmicroelectronics&logoColor=white"> <img src="https://img.shields.io/badge/raspberry%20pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white"> <img src="https://img.shields.io/badge/turtlebot3-22314E?style=for-the-badge&logo=ros&logoColor=white">

✅ 플랫폼 & 프레임워크

<img src="https://img.shields.io/badge/ROS-22314E?style=for-the-badge&logo=ros&logoColor=white"> <img src="https://img.shields.io/badge/flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white"> <img src="https://img.shields.io/badge/openai-412991?style=for-the-badge&logo=openai&logoColor=white"> <img src="https://img.shields.io/badge/openapi-6BA539?style=for-the-badge&logo=openapiinitiative&logoColor=white">

✅ 빌드 & 개발 환경

<img src="https://img.shields.io/badge/cmake-064F8C?style=for-the-badge&logo=cmake&logoColor=white"> <img src="https://img.shields.io/badge/ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white">

---

## 🧩 시스템 구성도 (간략)

```plaintext
[사용자] ↓ 음성 인식 [ESP32 - WiFi] ←→ [Flask 서버(API)] ←→ [GPT-4 Turbo] ↓ 센서 입력 (온도/조도 등) [STM32, Arduino Mega] ↓ [알람 출력, 디스플레이 등]
```

---

## 📁 프로젝트 구조

```plaintext
project_MOMs_Cookie/
├── App/
│   └── calendar/                # 일정 관리 모듈
├── BUZZER/                      # 알람 기능 구현
├── GPT4_Turbo/                  # AI 비서 기능
├── sensor_led/                  # 센서 및 LED 제어 (STM32 기반)
├── wifi_module_arduinomega/     # Wi-Fi 통신 모듈 (Arduino Mega 기반)
├── 서버 및 브릿지(API)/
│   └── final/                   # API 서버 및 브릿지 구현
├── 시연영상/                    # 프로젝트 시연 영상
└── 회로도/                      # 하드웨어 회로도
```

---

## 📽️ 시연 영상

시연 영상은 [여기](https://github.com/k-tae/project_MOMs_Cookie/tree/main/%EC%8B%9C%EC%97%B0%EC%98%81%EC%83%81)에서 확인하실 수 있습니다.

---

## 📄 회로도

하드웨어 회로도는 [여기](https://github.com/k-tae/project_MOMs_Cookie/tree/main/%ED%9A%8C%EB%A1%9C%EB%8F%84)에서 확인하실 수 있습니다.

---

## 개발자
<div align="center">

|권태형(팀장)|이종범(부팀장)|임소연|김병성|
|:------:|:------:|:------:|:------:|
| <a href="https://github.com/k-tae"><img width="150px" style="max-width: 100%;" src="https://github.com/k-tae.png"></a> | <a href="https://github.com/whdqja1128"><img width="150px" style="max-width: 100%;" src="https://github.com/whdqja1128.png"></a> | <a href="https://github.com/imso01"><img width="150px" style="max-width: 100%;" src="https://github.com/imso01.png"></a> | <a href="https://github.com/kimbseong0814"><img width="150px" style="max-width: 100%;" src="https://github.com/kimbseong0814.png"></a> |

</div>

---

## 📬 문의

이슈를 통해 문의를 남겨주시거나, 각 개발자에게 직접 연락 바랍니다.
