# ubuntu_packages
 emulator 
  - 우분투 터치 관련 emulator patch 가 적용된 버전
  - tarball 문제로 mouse로 가능하도록 패치함.
 ubuntu-keyboard-ko 
  - 한글 키보드(korean-layout)가 추가된 ubuntu-keyboard packages
  - autopilot / test package는 제거한 압축파일
  - ubuntu-touch ota 버전에 따른  prebuilt packages(for armhf)
  - BQ / MEIZU / NEXUS PHONE에서 검증 됨.

# ubuntu-keyboard-ko 설치 방법 (ex - OTA11 설치)
  adb shell or phone teminal app in ubuntu phone을 이용해서 하기 경로의 파일을 download한다.
  
  ubuntu-keyboard-ko URL is 
   https://github.com/cherojeong/ubuntu_packages/blob/master/ubuntu-keyboard-ko/ubuntu-keyboard-ko-ota11.tar.gz
  
  IN PC
  $adb shell

  IN ADB SHELL

  $cd Downloads
  $wget https://github.com/cherojeong/ubuntu_packages/blob/master/ubuntu-keyboard-ko/ubuntu-keyboard-ko-ota11.tar.gz
  $tar zvxf ubuntu-keyboard-ko-ota11.tar.gz
  $cd ubuntu-keyboard-ko-ota11
  $sudo apt-get install hunspell-ko
  $sudo dpkg -i *.deb
 
  우분투 시스템 설정 메뉴에서 한글 키보드 설정 후 사용가능
    - 한글 맞춤법 검사.
    - 사용자 DB , WORD-PREDICTIONARY 지원.
    - 2벌식 자판(쿼티)
    
    한글 키보드 사용 대모 영상
    https://www.youtube.com/watch?v=-O1BHlm29l0
    
  
  
