# Twitter memo
## version 0.0.1
# 용어
1. id : Twitter User Identifier
1. name : Twitter User handle
#  기능
1.  트위터 유저 프로필 페이지에서 저장된 메모를 볼 수 있음
2.  트위터 유저 프로필 페이지에서, 확장프로그램을 클릭해서 나온 팝업 창을 통해 메모를 추가할 수 있음
## 구현
1.  background
    *   localStorage에 id: memo 쌍을 저장
1.  popup
    *   popup에서 현재 페이지의 사용자의 id를 content를 통해 얻어 와 name을 얻을 수 있음
    *   popup에서 background를 통해 현재 페이지의 사용자에게 메모를 남길 수 있음
        *   내용은 background를 통해 저장
    *   popup에서 저장된 메모의 리스트를 확인할 수 있음
1.  content
    *   현재 페이지에서 css selector를 이용해 id를 얻음
    *   현재 페이지에 필요한 memo가 존재할 경우 페이지를 수정해서 프로필에 memo를 표시

1.  undefined 뜨는거 고치기 
1.  /home 방문 다음 프로필 페이지 방문 시 메모 미표시 오류
    *   head > script:nth-child(50) 오류 해결하기 
##    미구현

1.  popup에서 메모 리스트 확인하기
1.  popup에서 메모 삭제하기
1.  플러그인에서 새로고침 머시기
