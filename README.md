# 전주비전대 Project

## Install DHT11 sensor
```
git clone https://github.com/adafruit/Adafruit_Python_DHT.git
cd Adafruit_Python_DHT
sudo python setup.py install
cd Adafruit_python_DHT/examples
```
   -run
   ```
    python AdafruitDHT.py 11 4
   ```
   
  ## 1.Repository의 GPS key를 더하기
```
curl -sL https://repos.influxdata.com/influxdb.key | sudo apt-key add -
```
  ## 2.Repository를 더하기
```
echo "deb https://repos.influxdata.com/debian stretch stable" | sudo tee /etc/apt/sources.list.d/influxdb.list
```
  ## 3.프로그램 설치
```
sudo apt update
sudo apt install influxdb
```
  ## 4.프로그램 실행
```
sudo service influxdb start
```
  ## 5.데이터베이스 만들기
```
>create database <데이터베이스이름>
```
```
확인 : show databases
```
  ## 1.Repository의 GPS key를 더하기
  ```
  curl https://bintray.com/user/downloadSubjectPublicKey?username=bintray | sudo apt-key add -
  ```
  
  ## 2.Repository를 더하기
  ```
  echo "deb https://dl.bintray.com/fg2it/deb stretch main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
  ```
  
  ## 3.프로그램 설치
  ```
  sudo apt update
  sudo apt install grafana
  ````
  ## 4.프로그램 실행
```
sudo service influxdb start
```
  ### Git Hub Use
    - Repository down load
  ```
  git clone https://github.com/<username>/<repository name>
  ```
  ### vim editor setting
  ```
  set nu                // Line number
  set cindent          // C language indent
  set ts=4            // tab size 4
  if has("syntax")   // syntax on
      syntax on
  endif
  ```  
  
   ## VNC 서버
   ```
   vncserver
   ```
   ## 라즈베리 설정
   ```
   sudo raspi-config
   ```
   ## 뒤로가기
   ```
   cd ..
   ```
   ## 폴더 들어가기
   ```
   cd 폴더이름
   ```
   ## 현재 경로 파일 리스트
   ```
   ls
   ```
   ## 현재 경로 파일 리스트 및 권한, 크기, 날짜
   ```
   ls -al
   ```
   ## 직전에 있던 폴더 가는 방법
   ```
   cd -
   ```
   ## 현재 디렉토리
   ```
   ./
   ```
   ## 파일 복사
   ```
   cp 복사할파일 복사할위치
   ```
   ## 파일 삭제
   ```
   rm 삭제할 파일 -rf
   ```
   ## 리눅스 사용방법 기초
   ```
   bin   // 실행 파일 모음
   tmp   // 임시파일
   home  // user 폴더
   sbin  // 시스템 관리용 실행 파일
   usr   // 각종 프로그램
   root  // root home 디렉토리
   var   // 로그, 시스템 운영중 갱신데이터 저장
   lib   // 각종 라이브러리 설치되는 폴더
   ```
  ## 재부팅
   ```
   sudo reboot
   ```
   ## 라즈베리파이 설정 변경 - Bluetooth disable
   ```
   Bluetooth disable
   ```
  ## 이산화탄소
  ```
  #!/usr/bin/python
  
  import sys, serial, time
  
  comm = '/dev/ttyAMA0'
  baudrate = 38400
  
  device = serial.Serial(comm, baudrate, timeout = 5)
  print(device)
  
  while(True):
      try:
          rcvBuf = bytearray()
          device.reset_input_buffer()
          rcvBuf = device.read_until(size=12)
          print rcvBuf
      except Exception as e:
          print("Exception read") + str(e)
          
      time.sleep(5)
  ```
  ##타임봇
  ```
  vim timerbot.py
  ```
  ##python3 upgrade
  ```
  pip3 install python-telegram-bot --upgrade
  ```   
  ## telegrame-bot
  ```
  git clone https://github.com/python-telegram-bot/python-telegram-bot --recursive
  ```
