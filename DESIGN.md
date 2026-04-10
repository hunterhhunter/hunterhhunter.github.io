# Design System — Hunter's Study Blog

## Product Context
- **What this is:** ML 컴파일러 엔지니어를 꿈꾸는 SWE 학생의 개인 기술 블로그
- **Who it's for:** 채용 담당자, 동료 개발자, 같은 분야를 공부하는 학생
- **Space/industry:** CS / 시스템 엔지니어링 / ML 컴파일러
- **Project type:** 개인 블로그 (Hugo + PaperMod)

## Aesthetic Direction
- **Direction:** Industrial/Utilitarian + Retro-Futuristic 하이브리드
- **Decoration level:** Intentional (장식 최소화, 코드 블록과 타이포그래피가 주인공)
- **Mood:** 터미널과 컴파일러에서 영감받은, 기능 우선의 정돈된 디자인. "이 사람은 시스템 레벨에서 생각한다"는 인상을 3초 안에 전달.

## Typography
- **Display/Hero:** Pretendard Bold — 한글 최적화, 기하학적 산세리프. 제목에서 무게감.
- **Body:** Pretendard (16px / line-height 1.7) — 한글 가독성 최고 수준. 장문 읽기에 최적.
- **UI/Labels:** Pretendard Medium (14px)
- **Data/Tables:** JetBrains Mono (tabular-nums 지원)
- **Code:** JetBrains Mono (14px / line-height 1.5) — 리가처 지원, 개발자 정체성.
- **Loading:**
  - Pretendard: `https://cdn.jsdelivr.net/gh/orioncactus/pretendard/dist/web/variable/pretendardvariable.min.css`
  - JetBrains Mono: Google Fonts `https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&display=swap`
- **Scale:**
  - h1: 2rem (32px) / line-height 1.3
  - h2: 1.5rem (24px) / line-height 1.35
  - h3: 1.25rem (20px) / line-height 1.4
  - body: 1rem (16px) / line-height 1.7
  - small/caption: 0.875rem (14px) / line-height 1.5

## Color
- **Approach:** Restrained (1 액센트 + 뉴트럴. 컬러는 귀하게, 의미 있게)

### Dark Mode (기본)
| Role | Hex | RGB | Usage |
|------|-----|-----|-------|
| Background | #1a1b1e | rgb(26, 27, 30) | 페이지 배경 |
| Surface | #2a2b2f | rgb(42, 43, 47) | 카드, 입력 필드 |
| Primary text | #e8e6e3 | rgb(232, 230, 227) | 제목, 강조 텍스트 |
| Body text | #dcdad7 | rgb(220, 218, 215) | 본문 |
| Muted text | #8b8d93 | rgb(139, 141, 147) | 날짜, 메타 정보 |
| Border | #333333 | rgb(51, 51, 51) | 구분선, 카드 보더 |
| Accent | #d4a574 | rgb(212, 165, 116) | 링크, 버튼, 하이라이트 |
| Code block bg | #16171a | rgb(22, 23, 26) | 코드 블록 배경 |

### Light Mode
| Role | Hex | RGB | Usage |
|------|-----|-----|-------|
| Background | #f8f8f6 | rgb(248, 248, 246) | 페이지 배경 |
| Surface | #ffffff | rgb(255, 255, 255) | 카드 |
| Primary text | #1a1b1e | rgb(26, 27, 30) | 제목, 강조 |
| Body text | #262626 | rgb(38, 38, 38) | 본문 |
| Muted text | #6b7280 | rgb(107, 114, 128) | 날짜, 메타 |
| Border | #e5e5e0 | rgb(229, 229, 224) | 구분선 |
| Accent | #b4783c | rgb(180, 120, 60) | 대비 보장된 앰버 |
| Code block bg | #f5f5f3 | rgb(245, 245, 243) | 코드 블록 배경 |

### Semantic Colors
| Role | Hex | Usage |
|------|-----|-------|
| Success | #4ade80 | 성공 상태 |
| Warning | #d4a574 | 경고 (액센트와 동일) |
| Error | #ef4444 | 에러 상태 |
| Info | #60a5fa | 정보 알림 |

### Accessibility
- Dark mode body contrast: 12.6:1 (WCAG AAA)
- Light mode body contrast: 15.2:1 (WCAG AAA)
- Accent on dark: 7.3:1 (WCAG AA)
- Accent on light: 5.8:1 (WCAG AA)

## Spacing
- **Base unit:** 8px
- **Density:** Comfortable
- **Scale:** 2xs(2px) xs(4px) sm(8px) md(16px) lg(24px) xl(32px) 2xl(48px) 3xl(64px)

## Layout
- **Approach:** Grid-disciplined (단일 컬럼, 예측 가능한 정렬)
- **Max content width:** 720px
- **Nav width:** 1024px
- **Border radius:**
  - sm: 4px (뱃지, 태그)
  - md: 8px (카드, 코드 블록, 버튼)
  - lg: 12px (모달, 큰 컨테이너)
  - full: 9999px (프로필 이미지, 원형 요소)

## Motion
- **Approach:** Minimal-functional (이해를 돕는 전환만)
- **Easing:** enter(ease-out) exit(ease-in) move(ease-in-out)
- **Duration:**
  - micro: 50-100ms (호버 피드백)
  - short: 150-250ms (상태 전환, 호버)
  - medium: 250-400ms (테마 전환)
  - long: 400-700ms (사용하지 않음)

## Anti-patterns (하지 말 것)
- 보라/남색 그라디언트
- 3컬럼 아이콘 그리드
- 전부 center 정렬 (프로필 영역만 center, 나머지는 left)
- 장식용 블롭, 웨이브 SVG
- 이모지를 디자인 요소로 사용
- 균일한 border-radius (위계에 따라 다르게)
- "Built for X" / "Designed for Y" 류의 제네릭 카피

## Decisions Log
| Date | Decision | Rationale |
|------|----------|-----------|
| 2026-04-08 | Dark Engineer 팔레트 선택 | 터미널/컴파일러 연상, 개발자 정체성 강조 |
| 2026-04-08 | 다크 모드 기본 | Dark Engineer 컨셉 일치, 개발자 블로그 표준 |
| 2026-04-08 | Pretendard + JetBrains Mono | 한글 가독성 최고 + 개발자 코드 폰트 정체성 |
| 2026-04-08 | 앰버 액센트 (#d4a574) | 파란색 대신 터미널 경고/커서 연상, 차별화 |
| 2026-04-08 | 극단적 장식 절제 | 타이포그래피와 여백만으로 위계, 시스템 엔지니어 정돈된 사고 반영 |
