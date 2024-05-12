# 레이아웃 기본사항

Compose는 다음을 통해 상태를 UI 요소로 변환합니다.
> 컴포지션 &rarr; 레이아웃 &rarr; 드로잉

## 컴포즈 레이아웃 목표
고성능, 쉬운 레이아웃 작성
> **참고:** 뷰 시스템의 중첩 뷰는 성능상 문제가 있음, compose는 중첩에 성능에 영향이 없음

## 구성 가능한 함수
@Composable 함수는 기본 요소

## 레이아웃 구성요소
![레이아웃](https://developer.android.com/static/develop/ui/compose/images/layout-column-row-box.svg?hl=ko)

레이아웃 내 구성 요소 위치
Row
- horizontalArrangement
- verticalAlignment

Column
- verticalArrangement
- horizontalAlignment

## 레이아웃 모델
UI 트리 구성 : 각 노드 측정 요청, 하위 요소 없으면 크기 지정 및 배치, 하위요소에 있으면 하위 요소에 반복 요청
![레이아웃 모델](https://developer.android.com/static/develop/ui/compose/images/search-result-layout.svg?hl=ko)

## 성능
- 하위 요소 한번만 측정하여 높은 성능
