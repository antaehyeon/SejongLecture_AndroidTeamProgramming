세종대학교 모바일 프로그래밍 프로젝트 기술정리
==============================================

프로젝트를 진행하면서 겪었던 기술들에 대한 정리를 기록할 예정입니다.
--------------------------------------------------------------------

### 기술관련

-	MainActivity
	-	액션바 없애기

```
  ActionBar actionBar = getSupportActionBar();
  actionBar.hide();
```

-	imageView 에서 이미지 꽉 차게 하는법

```
  src로 경로를 지정하는 대신 background 속성을 이용하면 됨
```

-	colorCode - webCode

```
  Color.parseColor("color WEBCODE")
  ex) Color.parseColor("#FFFFFF")
  단, minSDK 21 이상
```

-	[TableLayout](http://recipes4dev.tistory.com/138)

```
  TableLayout - TableLow 구조를 가짐
  TableLow(행) 태그 안에 추가되는 요소들의 갯수(열) 구조
```

-	안드로이드 이미지 관련 이슈

```
  각 TableLayout 안에 있는 ImageView에 이미지를 설정하니
  맨 위의 이미지 뷰가 아래쪽의 이미지뷰를 전부 침범하는 문제가 발생
  이방법 저방법 다 써보다가 결국 layout_height=150dp로 설정
  그래도 상위 TableRow의 비율이 설정되어 있어서인지 각 핸드폰마다의 비율은 일정하게 설정됨
```

-	안드로이드 View 그림자 효과

```
  android:elevation="dp"
  android:translationZ="1dp"
```

-	[엘리베이션과 그림자](http://davidhyk.github.io/google-design-ko/what-is-material/elevation-shadows.html#)
