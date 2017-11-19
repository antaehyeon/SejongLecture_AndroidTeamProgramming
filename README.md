# 세종대학교 모바일 프로그래밍 프로젝트 기술정리

## 프로젝트를 진행하면서 겪었던 기술들에 대한 정리를 기록할 예정입니다.

### 기술관련
* MainActivity
  * 액션바 없애기
  ~~~~
  ActionBar actionBar = getSupportActionBar();
  actionBar.hide();
  ~~~~
  * imageView 에서 이미지 꽉 차게 하는법
  ~~~~
  src로 경로를 지정하는 대신 background 속성을 이용하면 됨
  ~~~~
