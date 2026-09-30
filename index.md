---
title: AI Token Tracker — Support
---

# AI Token Tracker — Support

AI Token Tracker is a macOS menu bar app that shows how much of your AI subscription quota (Claude, ChatGPT/Codex, Gemini CLI, Grok, Kimi, Qwen, Z.ai, Jev) is left this session and this week, using the sign-ins of the command-line tools already on your Mac.

- **Privacy policy:** [privacy](./privacy)
- **Questions, bugs, feature requests:** [open an issue](https://github.com/chb6734/aitokentracker-support/issues) — please include your macOS version, the app version (Settings › About) and which AI tools you are signed in to. Never paste tokens or API keys.

## Frequently asked questions

**Why does the app ask for access to my home folder?**
The app is sandboxed (Mac App Store). Your AI tools keep their sign-in files in your home folder (for example `~/.claude`, `~/.codex`, `~/.gemini`), and a sandboxed app can only read them after you allow it once in the system open panel. The access is read-only and can be revoked in Settings › Accounts.

**An account says the CLI's token has expired.**
The app never refreshes a CLI's login (doing so would log the CLI out). The message goes away by itself the next time you use that CLI; the last known usage stays visible meanwhile.

**Nothing was detected.**
Sign in with the tool's own CLI first (`claude`, `codex`, `gemini`, …), then use "Detect Again…" in Settings › Accounts. Providers with an API key or token can also be connected manually.

**Gemini shows "no longer serves this account".**
Since June 2026 Gemini CLI only serves Google Code Assist Standard/Enterprise accounts; consumer Google accounts are not supported by Google's endpoint.

## Data

The app has no server and collects nothing. Sign-in credentials are used only to ask the provider that issued them for your usage. Details: [privacy policy](./privacy).

---

# AI Token Tracker — 지원

AI Token Tracker는 이 Mac에 이미 로그인된 AI 명령줄 도구를 이용해 AI 구독(Claude, ChatGPT/Codex, Gemini CLI, Grok, Kimi, Qwen, Z.ai, Jev)의 이번 세션·이번 주 잔여량을 메뉴 막대에 보여주는 macOS 앱입니다.

- **개인정보 처리방침:** [privacy](./privacy)
- **문의, 버그, 기능 요청:** [이슈 남기기](https://github.com/chb6734/aitokentracker-support/issues) — macOS 버전, 앱 버전(설정 › 정보), 로그인한 AI 도구를 함께 적어 주세요. 토큰이나 API 키는 절대 붙이지 마세요.

## 자주 묻는 질문

**왜 홈 폴더 접근을 허용해야 하나요?**
앱은 Mac App Store용 샌드박스 안에서 동작합니다. AI 도구의 로그인 파일은 홈 폴더(예: `~/.claude`, `~/.codex`, `~/.gemini`)에 있고, 샌드박스 앱은 시스템 열기 패널에서 한 번 허용해야 읽을 수 있습니다. 읽기 전용이며 설정 › 계정에서 언제든 해제할 수 있습니다.

**계정에 "CLI 로그인 토큰이 만료되었습니다"라고 뜹니다.**
앱은 CLI의 로그인을 대신 갱신하지 않습니다(갱신하면 CLI가 로그아웃됩니다). 해당 CLI를 다시 사용하면 자동으로 사라지고, 그동안 마지막 사용량이 유지됩니다.

**감지된 계정이 없습니다.**
먼저 도구의 CLI(`claude`, `codex`, `gemini` 등)로 로그인한 뒤 설정 › 계정의 "다시 찾기"를 누르세요. API 키나 토큰이 있는 제공자는 직접 연결할 수도 있습니다.

**Gemini에 "더 이상 서비스하지 않음"이 표시됩니다.**
2026년 6월부터 Gemini CLI는 Google Code Assist Standard/Enterprise 계정만 지원하며, 일반 소비자 Google 계정은 Google 쪽에서 지원하지 않습니다.
