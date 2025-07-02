# 💸 후원 자막 설정 방법

## 1. 커스텀 스타일 CSS 적용

먼저 **후원 자막 스타일**을 커스터마이징하기 위해 **커스텀 스타일 CSS 사용**을 누른 후 다음 코드를 복사해 붙여넣어주세요:

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

---

## 2. 후원 자막 종류 설정

- 자막 종류: `mvp`  
※ 이 종류에 CSS 스타일이 적용됩니다.

---

## 3. 자막 텍스트 입력 방식

자막에 표시될 텍스트는 다음 형식으로 입력해주세요:

```
From. {닉네임}님 {금액}
```

### 예시:
```
From. 홍도유님 5,000원
```

---

✅ 위 설정대로 적용하면 자막 앞에 후원 아이콘이 표시되고, 흰색 배경 + 하트가 포함된 스타일이 적용됩니다.
