# 환경설정

- 초기 프로젝트 생성시 additional option에서 Precompiled Header 사용하면 다른 OS로 변환시 문제될 수 있다.
- solution 아래에 여러 프로젝트가 있을 경우, 프로젝트별로 실행하고 싶다면 프로젝트 우클릭 -> set as startup project 로 실행할 project 를 변경할 수 있다. Bold 체로 어떤 프로젝트가 실행될지 알 수 있다.
- 파일을 실행하여 콘솔 출력 후 바로 사라지면 properties - linker - system - subsystem 을 console로 변경해본다.