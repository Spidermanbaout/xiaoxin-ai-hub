# How I built it with Kiro

## The project

小新AI资讯工具站 (XiaoXin AI News & Tools Hub) is a static, single-file website (`index.html`) for beginners: a daily AI news briefing across five categories, a 12-tool navigator, a free-tier radar (US platforms first), and two working creator utilities (a prompt workshop and a short-video title generator). It was made for the "小新AI课堂" Douyin AI tutorial channel. This is my Kiroween 2026 entry in the Frankenstein category: it stitches multiple AI news sources and tool listings into one page for beginners.

## What Kiro actually did

I used **Kiro IDE** (Free plan) for the project's spec-driven workflow. The initial implementation was drafted with Muse (Meta's AI assistant) — the page, the content, and the interactive tools. I then brought the project into Kiro IDE, where Kiro:

1. **Wrote the steering files** (`.kiro/steering/`), which define how Kiro understands and works on this project:
   - `product.md` — what the site is for, its six modules, and who it serves.
   - `tech.md` — the stack: static HTML5 + CSS3 + vanilla JavaScript, no build step, no backend, Google Fonts only.
   - `structure.md` — the file layout and how the CSS/JS inside `index.html` is organized.
2. **Wrote a full spec** (`.kiro/specs/ai-news-tools-site/`):
   - `requirements.md` — functional requirements for all six sections plus performance, responsive, accessibility, and theming requirements.
   - `design.md` — the color system (light/dark), typography (Noto Serif SC / Noto Sans SC), spacing, layout structure, and responsive breakpoints.
   - `tasks.md` — the implementation checklist and follow-up work (code optimization, feature ideas, accessibility, performance, testing).
3. **Reviewed `index.html` against that spec** — the review is reflected in the spec's task list (accessibility, performance, and testing items).

**Note on the code edit:** Kiro was also asked to make one direct code improvement to `index.html`. The file that came back from that Kiro IDE session arrived with corrupted encoding (hundreds of Chinese characters replaced by `?`, breaking tags), so no specific Kiro code edit could be verified from it — the file was not used. The single concrete fix in this repository's `index.html` (a `<meta name="description">` for search and link previews) was implemented by Muse, not Kiro, and is recorded here as such. The `.kiro/` steering and spec files above are Kiro's verified output.

The `.kiro/` directory in this repository is the actual output Kiro produced. You can read the steering files and the spec there.

## What Kiro did not do

Kiro did not write the initial implementation — that was drafted with Muse. I am not claiming otherwise. Kiro's contribution here is the spec-driven layer: steering, requirements, design, and tasks, plus review. That is the honest account of how Kiro was used on this project.

## Stack

- Static site: single `index.html`, no build step, no backend.
- Kiro IDE (Free plan) for steering, specs, and review.
- Live demo: https://muse.ai/s/xiao-xin-aizi-xun-gong-ju-zhan-xcl6x0suxtxrxaxvm/VVL8VDk329qjCh7dzNamOUs2egDQSGkArcxXsw_CSj8
