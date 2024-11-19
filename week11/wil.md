## 11주차 스터디 강의 요약
# Relation과 FK
Relation(관계)   
1:1 
1:다 - FK를 이용하여 두 테이블을 하나씩 연결한다. '다' 쪽의 테이블이 FK를 가진다   
다:다 - 보조 테이블을 이용하여 연결한다.
FK(ForeignKey)   
클래스 멤버 변수에 models.ForeignKey()를 사용하여 FK를 추가한다.   
on_delete는 연결된 항목이 삭제되었을 경우, 해당 테이블의 FK column을 어떻게 할 것인가 설정하는 항목이다.   
on_delete에는 여러 속성들을 지정할 수 있다.   
1. Models.CASCADE: 외래키로 연결된 항목이 삭제되면 해당 항목도 같이 삭제
2. Models.PROTECT: FK로 연결된 항목은 삭제할 수 없도록 삭제시도 시 오류를 띄워준다.   

