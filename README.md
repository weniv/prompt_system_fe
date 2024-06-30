# prompt_system_fe

위니브의 디자인 시스템을 프롬프트로 만든 프롬프트 디자인 시스템

## 목적

- FE 분들의 빠른 웹 페이지 작업
- 일관성 있는 디자인 시스템 제공

## 방향성

1. 위니브의 디자인 시스템을 tailwind css로 직접 코드 작성
2. 위니브의 디자인 이미지를 클라우드에 업로드
3. 프롬프트로 header, main, card, footer 등을 입력하고 원하는 스타일 지정
4. 기본으로 신경써야 했던 다양한 노하우를 프롬프트로 제공, 아래 5가지 말고도 추후 추가 예정
   4.1 검색엔진 최적화해서 코드를 짜줘
   4.2 접근성을 고려해서 코드를 짜줘
   4.3 반응형으로 코드를 짜줘
   4.4 화이트, 다크테마가 변경가능하도록 코드를 짜줘
   4.5 브라우저 호환성을 고려해서 코드를 짜줘

## 시도했던 여러 실패 기록

- figma to code로 tailwind css로 변환
  - 만족스럽지 못한 결과물(주니어 수준도 안됨)
- claude의 html 소스코드를 html to figma로 변환
  - 만족스럽지 못한 결과물(주니어 수준도 안됨)
- claude에서 이미지 인식, PDF 인식, SVG 인식
  - 만족스럽지 못한 결과물(주니어 수준도 안됨)
- 여러 툴을 조사했었으나 유료 서비스도 결국 주니어 수준(이미지 참고)

## 입력했던 프롬프트

회사에서는 직원이 입사할 때마다 캐릭터를 그려. 전체 캐릭터 이미지는 `https://github.com/weniv/weniv_friends_design_asset/blob/main/%ED%94%84%EB%A0%8C%EC%A6%88%EC%A0%84%EC%B2%B4/2024.png?raw=true`이야. 이미지 크기는 3792 x 2166이야.

404페이지는 `https://github.com/weniv/weniv_friends_design_asset/blob/main/etc/404.png?raw=true`이야. 이미지의 크기는 300에 240이야.

default 이미지는 `https://github.com/weniv/weniv_friends_design_asset/blob/main/etc/default.png?raw=true`이야. 이미지 크기는 760에 400이야.

배경 이미지는 `https://github.com/weniv/weniv_friends_design_asset/blob/main/%EC%A4%8C%20%EB%B0%B0%EA%B2%BD/1.png?raw=true`이야. 이미지 크기는 3840에 2160이야.

logo 이미지는 `https://github.com/weniv/weniv_friends_design_asset/blob/main/etc/weniv_logo.png?raw=true`이야. 이미지 크기는 1857에 429야.

세로로 길죽한 형태, 엽서 형태로 사용할 수 있는 이미지 목록은 아래와 같아. 모두 501에 701로 되어 있어.

1. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-02.webp?raw=true`
2. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-04.webp?raw=true`
3. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-06.webp?raw=true`
4. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-08.webp?raw=true`
5. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-10.webp?raw=true`
6. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-12.webp?raw=true`
7. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-14.webp?raw=true`
8. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-16.webp?raw=true`
9. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-18.webp?raw=true`
10. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-20.webp?raw=true`
11. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/-22.webp?raw=true`

가로와 세로 비율이 적당한 형태, 직사각형 형태로 사용할 수 있는 이미지 목록은 아래와 같아. 모두 935에 701로 되어 있어.

1. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/1.webp?raw=true`
2. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_friends/2.webp?raw=true`

프로필로 사용할 수 있는 이미지 목록은 아래와 같아. 이미지 배율이 제목에 있어.

1. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/53x100_1.png?raw=true`
2. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/53x100.png?raw=true`
3. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/54x100.png?raw=true`
4. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/61x100.png?raw=true`
5. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/67x100_1.png?raw=true`
6. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/67x100.png?raw=true`
7. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/70x100.png?raw=true`
8. `https://github.com/weniv/weniv_friends_design_asset/blob/main/weniv_profile/73x100.png?raw=true`

이 이미지를 가지고 인스타그램 클론 코딩을 해줘.

1. tailwind를 사용해줘.
2. 이미지는 배율이 깨지지 않도록 해줘. 특히 프로필 사진이 배율이 깨지지 않아야해.
3. 최 상단에는 친구들 릴스를 볼 수 있는 공간이 있어. 클릭이 되었을 때 실제 동작될 필요는 없어. 이건 나중에 구현할 예정이야.
4. 중간에는 친구들의 포스팅을 볼 수 있는 공간이 있어. 클릭이 되었을 때 실제 동작될 필요는 없어. 이건 나중에 구현할 예정이야.
5. 포스팅에 좋아요 정도는 클릭이 가능하게 해줘.
6. 왼쪽에는 인스타그램 로고와 함께 홈, 검색, 탐색 탭, 릴스, 메시지, 알림, 만들기, 프로필이 모여있는 공간이 있어. 클릭이 되었을 때 실제 동작될 필요는 없어. 이건 나중에 구현할 예정이야.
7. 코드를 짤 때 SEO를 고려해줘.
8. 코드를 짤 때 웹 접근성을 고려해줘.
