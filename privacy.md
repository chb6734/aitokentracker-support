---
title: AI Token Tracker — Privacy Policy
---

# Privacy Policy — AI Token Tracker

_Last updated: 2026-09-29_

AI Token Tracker is a macOS menu bar app that shows how much of your AI subscription quota is left. It is made by an individual developer (Hyunbin Cha). This policy explains what the app reads, where that data goes, and what it never does.

## What the app does not do

- It does **not** collect, transmit or store any data on servers run by the developer. There is no backend.
- It contains **no analytics, tracking, advertising or crash-reporting** SDKs. The app has no third-party dependencies.
- It never writes to the files of other apps or tools, and never changes your sign-in state in any AI tool.

## What the app reads on your Mac

The app runs inside the macOS App Sandbox. To find the AI accounts you are signed in to, it asks you once to allow read access to your home folder. With that permission it reads, **read-only**:

- the local sign-in files of AI command-line tools (for example `~/.claude`, `~/.codex`, `~/.gemini`, `~/.grok`, `~/.kimi`, `~/.qwen`, `~/.config/jev`), and, for Claude Code, its Keychain item (macOS asks for your confirmation the first time);
- those tools' local log folders, to show token totals and to refresh usage promptly while you work.

You can revoke this permission at any time in Settings › Accounts. Without it, the app can only track accounts whose API key or token you paste in manually.

## Where the data goes

- A sign-in credential is used for exactly one purpose: asking **the provider that issued it** (Anthropic, OpenAI, Google, xAI, Moonshot AI, Alibaba Cloud, Zhipu AI or TypeSafe) for your current usage. It is sent only to that provider's own servers over HTTPS, and never to anyone else.
- The app also polls the providers' public status pages (for example `status.claude.com`) to show service incidents. These requests carry no account data.
- Nothing is sent to the developer.

## What the app stores locally

- Credentials you connected are kept in your macOS Keychain, under this app's own service, readable only by this app.
- Usage snapshots, a short usage history and your settings are kept in the app's sandbox container (`~/Library/Containers/…/Data/Library/Application Support/AI Token Tracker/`).
- Removing an account in Settings deletes its Keychain item and its usage history. Deleting the app removes the container.

## Your choices

- Accounts found signed in are connected automatically once you allow home folder access (Claude Code's Keychain login also without it). Turn tracking off per account or remove an account at any time in Settings › Accounts; removing deletes its stored credential and history.
- Revoke home folder access at any time in Settings.

## Contact

Questions about this policy: open an issue at <https://github.com/chb6734/aitokentracker-support/issues> (support page: <https://chb6734.github.io/aitokentracker-support/>).

---

# 개인정보 처리방침 — AI Token Tracker

_최종 수정: 2026-09-29_

AI Token Tracker는 AI 구독의 남은 사용량을 메뉴 막대에 보여주는 macOS 앱입니다. 개인 개발자(차현빈)가 만들었습니다. 이 문서는 앱이 무엇을 읽고, 그 데이터가 어디로 가며, 무엇을 절대 하지 않는지 설명합니다.

## 앱이 하지 않는 것

- 개발자가 운영하는 서버로 데이터를 **수집·전송·저장하지 않습니다.** 백엔드가 없습니다.
- **분석, 추적, 광고, 크래시 리포트 SDK가 없습니다.** 외부 의존성이 없습니다.
- 다른 앱이나 도구의 파일에 쓰지 않으며, 어떤 AI 도구의 로그인 상태도 바꾸지 않습니다.

## 앱이 이 Mac에서 읽는 것

앱은 macOS App Sandbox 안에서 동작합니다. 로그인된 AI 계정을 찾기 위해 홈 폴더 읽기 권한을 한 번 요청합니다. 허용하면 다음을 **읽기 전용**으로 읽습니다.

- AI 명령줄 도구의 로컬 로그인 파일(예: `~/.claude`, `~/.codex`, `~/.gemini`, `~/.grok`, `~/.kimi`, `~/.qwen`, `~/.config/jev`)과, Claude Code의 경우 Keychain 항목(처음 한 번 macOS가 확인을 요청합니다)
- 위 도구들의 로컬 로그 폴더(토큰 합계 표시, 작업 중 빠른 갱신)

이 권한은 설정 › 계정에서 언제든 해제할 수 있습니다. 해제하면 API 키나 토큰을 직접 입력한 계정만 추적할 수 있습니다.

## 데이터가 가는 곳

- 로그인 정보는 오직 한 가지 목적, 즉 **그 로그인을 발급한 제공자**(Anthropic, OpenAI, Google, xAI, Moonshot AI, Alibaba Cloud, Zhipu AI, TypeSafe)에게 현재 사용량을 묻는 데만 쓰입니다. HTTPS로 해당 제공자의 서버에만 전송되며 다른 곳으로는 절대 보내지 않습니다.
- 서비스 장애 표시를 위해 제공자의 공개 상태 페이지(예: `status.claude.com`)도 조회합니다. 이 요청에는 계정 정보가 담기지 않습니다.
- 개발자에게는 아무것도 전송되지 않습니다.

## 로컬에 저장하는 것

- 연결한 자격증명은 이 앱 전용 서비스 이름으로 macOS Keychain에 저장되며 이 앱만 읽을 수 있습니다.
- 사용량 스냅샷, 짧은 사용량 기록, 설정은 앱의 샌드박스 컨테이너(`~/Library/Containers/…/Data/Library/Application Support/AI Token Tracker/`)에 저장됩니다.
- 설정에서 계정을 제거하면 Keychain 항목과 사용량 기록이 삭제됩니다. 앱을 삭제하면 컨테이너가 제거됩니다.

## 선택권

- 홈 폴더 접근을 허용하면 로그인된 계정이 자동으로 연결됩니다(Claude Code의 Keychain 로그인은 허용 없이도 연결). 설정 › 계정에서 계정별로 추적을 끄거나 계정을 제거할 수 있으며, 제거하면 저장된 자격증명과 기록이 삭제됩니다.
- 설정에서 홈 폴더 접근을 언제든 해제할 수 있습니다.

## 문의

<https://github.com/chb6734/aitokentracker-support/issues>에 이슈를 남겨 주세요 (지원 페이지: <https://chb6734.github.io/aitokentracker-support/>).
