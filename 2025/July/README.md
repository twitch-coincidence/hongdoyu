# 💬 기본 채팅창 설정 방법

## 1. 테마 설정

- 테마: **기본**
- 채팅 정렬: **한 줄**
- 커스텀 스타일 CSS: **사용으로 체크**하고 아래 코드 복사해서 붙여넣기

```css
.chat_box .inner_box {
	display: flex;
  	justify-content: center;
}

.icon_badge {
	width: 28px !important;
  	height: 28px !important;
}

.icon_badge.streamer {
	background: url(https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_streamer.webp);
  	background-size: 28px 28px !important;
}

.icon_badge.manager {
  	display: none;
}

.icon_badge.top {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_top.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.icon_badge.fan {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_fan.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.icon_badge.subscribe {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_subscribe.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.chat_box .nick {
	display: none;
}

.chat_box .text::before {
	content: "\"";
}

.chat_box .text::after {
	content: "\"";
}
```

## 2. 상세 설정

- **시청자 닉네임 표시**는 반드시 켜두세요  
  → 제가 CSS로 닉네임을 숨겨뒀으니 걱정 안 하셔도 됩니다.  
  다만 이 옵션이 꺼져 있으면 **아이콘이 표시되지 않습니다!**

## 3. 채팅 아이콘

- 전부 켜두시는 걸 추천드려요!

---

# 💛 카톡 테마 채팅창 설정 방법

## 1. 테마 설정

- 테마: **카카오톡**
- 테마 세부 설정:  
  - 카카오톡 채팅 정렬: **시청자만 왼쪽**  
  - 왼쪽 채팅 배경색: `#e7f5ff`  
  - 오른쪽 채팅 배경색: `#8c78aa`
- 커스텀 스타일 CSS: **사용으로 체크**하고 아래 코드 복사해서 붙여넣기

```css
.chat_box .inner_box {
	display: flex;
}

.chat_box.streamer .inner_box {
	flex-direction: row-reverse;
}

.icon_badge {
  	position: relative;
  	top: -15px !important;
	width: 28px !important;
  	height: 28px !important;
}

.icon_badge.streamer {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_streamer.webp") 50% 50% no-repeat !important;
  	background-size: 28px 28px !important;
}

.icon_badge.manager {
  	display: none;
}

.icon_badge.top {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_top.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.icon_badge.fan {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_fan.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.icon_badge.subscribe {
	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/chat_subscribe.webp") 50% 50% no-repeat !important;
	background-size: 28px 28px !important;
}

.chat_box .nick {
	display: none;
}
```

## 2. 상세 설정

- **시청자 닉네임 표시**는 반드시 켜두세요  
  → 제가 CSS로 닉네임을 숨겨뒀으니 걱정 안 하셔도 됩니다.  
  다만 이 옵션이 꺼져 있으면 **아이콘이 표시되지 않습니다!**

## 3. 채팅 아이콘

- 전부 켜두시는 걸 추천드려요!

---

# 💸 후원 자막 설정 방법

## 1. 테마 설정

- 테마: **기본**
- 커스텀 스타일 CSS: **사용으로 체크**하고 아래 코드 복사해서 붙여넣기

```css
.subtitle_area {
	display: flex;
  	align-items: center;
}

.subtitle_area::after {
	content: "";
   	display: block;
  	position: absolute;
  	background: url("https://raw.githubusercontent.com/twitch-coincidence/hongdoyu/refs/heads/main/2025/July/img/donation_icon.webp");
	background-size: 89.5px auto;
  	background-repeat: no-repeat;
  	width: 89.5px;
  	height: 70px;
}

.mvp {
	width: fit-content;
}

.text_box {
	background: #ffffffa5;
  	border-radius: 12px;
  	margin-left: 50px;
}

.mvp .text {
	padding-left: 45px;
  	padding-right: 12px;
}

.mvp .text::after {
  	margin-left: 5px;
	content: "🤍";
  	text-shadow: none;
}
```

## 2. 상세 설정

- **후원 자막 종류**: `MVP`
- 자막 텍스트:  
  `From. {nickname}님 {number}`
