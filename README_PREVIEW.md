# Design Architecture & Preview Specifications

This document outlines the architecture, color palette, responsive layout decisions, and service integrations for **Harish S's** GitHub Profile README.

---

## 🎨 Visual Identity & Design Tokens

| Property | Value | Rationale |
| :--- | :--- | :--- |
| **Theme** | Dark Developer Modern | Aligned with high-tier developer portfolios and GitHub Dark Default. |
| **Base Background** | `#0d1117` | Standard GitHub Dark canvas to blend seamlessly with stats widgets. |
| **Primary Accent** | `#00f2fe` / `#38bdf8` (Cyan & Sky Blue) | Clean, high-tech cybersecurity & intelligence vibe. |
| **Secondary Accent**| `#8b5cf6` (Electric Violet) | Highlights embedded systems, AI, and innovation engineering. |
| **Neutral Foreground**| `#c9d1d9` / `#ffffff` | High-contrast, recruiter-readable typography. |
| **Badge Style** | `for-the-badge` & `flat-square` | Flat, geometric, consistent padding and high visual clarity. |

---

## 📐 Layout & Hierarchy

1. **Header Section:**
   - Centered greeting with full professional identity and title.
   - Dynamic typing SVG banner showcasing core specialties:
     - *Cybersecurity Enthusiast • Network Forensics*
     - *Python Development • Security Automation*
     - *Embedded Systems • IoT • Computer Vision*
   - Profile view counter and specialty badges.
2. **About Me:**
   - Bulleted summary focusing on real areas of interest: cybersecurity, Python automation, embedded microcontrollers, computer vision, practical prototyping, and continuous learning.
3. **Categorized Skills Matrix:**
   - 2x2 responsive table categorized into:
     - *Cybersecurity & Networking*
     - *Programming & Web*
     - *AI & Computer Vision*
     - *Embedded Systems & IoT*
   - Badges use official brand icons and hex colors.
4. **Featured Projects:**
   - 2x2 + full-width grid using GitHub-compatible HTML tables.
   - Highlights 5 genuine repositories from [@Haridh432](https://github.com/Haridh432):
     - `Network-Triage`: Wireshark packet analysis, Python, PDF reporting.
     - `phishing-email-analyzer`: EML forensics, SPF/DKIM/DMARC checks.
     - `Sign-language-recognition`: OpenCV, MediaPipe, ASL gesture recognition.
     - `IoT`: Embedded C++, ESP32 sensor integration.
     - `My-Trickster`: Frontend design, HTML5, CSS3.
5. **Dynamic Statistics Dashboard:**
   - GitHub Overall Stats (`github-readme-stats` with custom `tokyonight` palette and `#0d1117` background).
   - Top Languages Breakdown.
   - Streak Counter (`streak-stats.demolab.com`).
6. **Current Focus & Connect Sections:**
   - Structured outlook on current engineering objectives.
   - Clean profile links and collaborative invitation for recruiters and open-source contributors.

---

## 🛡️ Compatibility & Security Notes

- **Zero JavaScript Execution:** Pure Markdown and HTML supported natively by GitHub's rendering engine.
- **No Private Tokens:** External stats are pulled purely using public username queries (`user=Haridh432`). No secret tokens or personal API keys are required or exposed.
- **Mobile Responsive:** All table column widths are specified using percentages (`50%`), ensuring fluid wrapping on smaller screens.
