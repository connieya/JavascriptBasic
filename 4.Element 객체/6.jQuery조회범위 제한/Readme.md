# jQuery 조회 범위 제한

이전 수업에서 Element 객체에서 getElementsBy\* 메소드를 실행하면 조회의 범위가 그 객체의
하위 엘리먼트로 제한된다는 것을 알아봤다. jQuery는 어떻게 이러한 작업을 할 수 있을까?

## selector context

가장 간편한 방법은 조회할 때 조회 범위를 제한하는 것이다. 그 제한된 범위를 jQuery에서는

selector context라고 한다.

## find()

find는 jQuery 객체 내에서 엘리먼트를 조회하는 기능을 제공한다.
