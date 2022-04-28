# Kokoa Clone 2022 Update

HTML & CSS are so much fun

# setting

뒤로가기 버튼 적용.

# chat screen

chat screen에서 이름 중앙 배치 -> position reletive 사용 left 17px

검색 아이콘과 bar아이콘 사이 간격 조정 -> margin-left

main에서 상대방의 말과 내 말 -> span 이용

내 말에서는 div안에 class를 하나 더 생성(message-row--own)

위치 바꾸기 -> html에서 span의 위치를 바꾸면 되지만, flex-direction: row-revers; 를 이용하여 위치 바꿈

input을 이용해서 보내기 창 만들기 -> form 이용

답장하기 창 에서 창 고정 -> position: fixed;

보내기 버튼과 이모티콘 아이콘을 input위에 올림 -> position: absolute;
중앙에 맞기 하나하나 적용

absolute는 부모에 reletive가 필요하므로 버튼과 이모티콘 아이콘의 부모인 reply_column:last-child 에 position: reletive; 사용

# 오류수정

chat.css에서 h1부분에 class 이름을 주지않고 선언, 모든 h1에서 오류 발생
-> h1이동(오른쪽)

해결 : chat.css 파일에서 h1부분 삭제 후, class 이름을 주고, class이름으로 다시
선언

reply input에서 padding: 12px; 로 설정 후, 이모티콘 아이콘과 보내기 버튼이 처음 위치보다 이동.

해결: 다시 이모티콘 아이콘과 보내기 버튼을 하나하나 이동.

# 이해X

box-sizing: border-box; ??

# 애니매이션

friends.html -> 카카오 시작배경 적용

내비게이션바 애니매이션 적용

chat 보내기 input창 애니매시션 적용

설정아이콘 마우스 hover -> 애니메이션 적용

forwards -> 끝나고 유지
@keyframes -> 애니매이션
