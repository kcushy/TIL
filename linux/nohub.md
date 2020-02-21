# nohub

- argument로 적은 명령을 hangup 신호 무시한 채 수행 가능하게 해준다. 

- nohub 파일명 &

  - 자동으로 백그라운드로 보내지 않기 때문에 &을 뒤에 붙여서 background로 실행

- 종료

  ```
  ps -ef
  kill -9 <실행파일에 해당하는 pid>
  ```

  