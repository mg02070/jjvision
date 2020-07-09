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
