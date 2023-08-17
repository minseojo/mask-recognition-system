# 프로젝트 계기 [스마트 패스]
covid-19로 우리 사회는 인력 부족에 시달렸다. 사물 인터넷(IOT)를 이용하여 도움을 보탤 방법은 없을까? <br>
라는 마음에 시작했다.

---
# 프로젝트 목적
1. 마스크 착용 유무 파악 (카메라 & 딥러닝)
2. 측정한 체온이 정상인지 판별
3. 두 가지 조건을 만족하였을 때 알림 구현(LED, 소리)

---
# 시스템 구성도 
![image](https://github.com/minseojo/mask-recognition-system/assets/64322765/d65aaf50-900e-4e67-91ca-559c91be9321)

## HW 구성 & 용도
1. wifi - 무선 와이파이 (인터넷 연결)
2. HDMI Monitor - 라즈베리 파이 화면 출력
3. 4 USB prots - 키보드, 마우스 입력포트
4. 5V Micro USB - 전원 
5. CSI Camera Connector - 카메라 연결
6. Micro SD card Slot - OS 및 S.W가 저장된 SD 카드 
7. 40pin GPIO Header - 5V(3 pin), Ground(1 pin), Signal(4 pin [temperature sensor]& 23 pin [Green LED], 24 pin [Red LED])

## SW 구성
1. 라즈비안 OS를 기반으로 Python 3.7 설치
2. 얼굴인식 구현에 필요한 라이브러리 (tensorflow, numpy, matplotlib, openCV) 설치
3. frame(마스크 쓴 모습)을 일정 시간마다 받아 함수에 전달한다.
4. frame을 받아 마스크 착용여부를 예측하는 함수 구현

---
# 기대 효과 및 활용 방안
1. 통행이 잦은 곳에 인건비보다 저렴한 스마트 패스를 둔다.
2. 인건비 절감
3. 인력 낭비를 줄여 일손이 필요한곳에 쓰인다.

---
# 결과
![image](https://github.com/minseojo/mask-recognition-system/assets/64322765/20deb5b6-00e6-4f3d-9401-097898588406)
제 얼굴이 아니라 가렸습니다. <br>

## CASE
1) 마스크를 썼을 때
	1-1) 정상체온일 때
	1-2) 정상체온보다 높을 때
2) 마스크를 쓰지 않았을 때
 	2-1) 체온을 판별하지 않음



