> 새로운 옵시디언 보관소(vault)를 만들 때, 기존에 쓰고있는 디자인을 유지하기 위함.

# 1. 이미지 경로 지정

옵시디언에 이미지를 복붙하면 최상위 root 경로에 이미지가 저장됩니다.
그거를 방지하기 위해서 새로운 폴더를 만들고 경로를 지정해줍니다.

1. 옵시디언 설정 -> 파일 및 링크 -> 새 첨부 파일을 만들 위치
2. `보관소의 최상위 폴더` -> `현재 폴더의 하위 폴더` 로 변경
3. 첨부 파일 폴더 경로를 `images`로 변경 
4. `[[wikilink]]` 체크 해제
![](Pasted%20image%2020241221062138.png)

# 2. 테마 변경

1. 옵시디언 설정 -> 테마 -> 테마 관리
2. `AnuPpuccin` 검색 후 설치


# 3. Style Settings 플러그인 설치

1. 옵시디언 설정 -> 커뮤니티 플러그인 -> 탐색
2. `Style Settings` 검색 후 설치
3. 설치 후 설정 -> 커뮤니티 플러그인 탭에 생긴 Style Settings 클릭
4. Obsidian 폴더에 있는 `color-extend.css` 파일 -> `.obsidian/snippets` 으로 이동
   (숨김 폴더/폴더 생성)
   `mkdir -p .obsidian/snippets && cp Obsidian/color-extend.css .obsidian/snippets/color-extend.css`
5. 옵시디언 설정 -> 테마 맨 하단 -> `CSS snippets`에 추가된 `color-extend` 활성화
6. Import로 아래 내용 붙여넣기

```Json
{
  "anuppuccin-theme-settings-extended@@anp-theme-ext-light": true,
  "anuppuccin-theme-settings-extended@@anp-theme-ext-dark": true,
  "anuppuccin-theme-settings-extended@@anp-theme-ext-amoled": true,
  "anuppuccin-theme-settings-extended@@catppuccin-theme-extended": "ctp-atom-light",
  "anuppuccin-theme-settings-extended@@catppuccin-theme-dark-extended": "ctp-generic-dark",
  "anuppuccin-theme-settings@@anp-active-line": "anp-current-line",
  "anuppuccin-theme-settings@@anp-callout-select": "anp-callout-block",
  "anuppuccin-theme-settings@@anp-callout-color-toggle": true,
  "anuppuccin-theme-settings@@anp-custom-checkboxes": true,
  "anuppuccin-theme-settings@@anp-speech-bubble": true,
  "anuppuccin-theme-settings@@anp-toggle-scrollbars": true,
  "anuppuccin-theme-settings@@anp-header-color-toggle": true,
  "anuppuccin-theme-settings@@anp-header-margin-toggle": true,
  "anuppuccin-theme-settings@@anp-decoration-toggle": true,
  "anuppuccin-theme-settings@@anp-canvas-dark-bg": true,
  "anuppuccin-theme-settings@@anp-colorful-frame-icon-toggle-dark": false,
  "anuppuccin-theme-settings@@anp-custom-vault-toggle": true,
  "anuppuccin-theme-settings@@anp-file-icons": true,
  "anuppuccin-theme-settings@@anp-alt-rainbow-style": "anp-simple-rainbow-color-toggle",
  "anuppuccin-theme-settings@@anp-simple-rainbow-title-toggle": true,
  "anuppuccin-theme-settings@@anp-simple-rainbow-collapse-icon-toggle": true,
  "anuppuccin-theme-settings@@anp-simple-rainbow-indentation-toggle": true,
  "anuppuccin-theme-settings@@anp-simple-rainbow-icon-toggle": true,
  "anuppuccin-theme-settings@@anp-layout-select": "anp-card-layout",
  "anuppuccin-theme-settings@@anp-floating-header": false,
  "anuppuccin-theme-settings@@anp-rainbow-subfolder-color-toggle": false,
  "anuppuccin-theme-settings@@anp-rainbow-file-toggle": false,
  "anuppuccin-theme-settings@@anp-full-rainbow-text-color-toggle-light": false,
  "anuppuccin-theme-settings@@anp-full-rainbow-text-color-toggle-dark": false,
  "anuppuccin-theme-settings@@anp-status-bar-select": "none",
  "anuppuccin-theme-settings@@anp-alt-tab-style": "anp-default-tab"
}
```
