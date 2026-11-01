---
name: "ned-academy-course-banner"
description: "Create an NED Academy course banner/flyer for a new course; collect all needed details through multiple-choice forms, then build the standard layout."
---

# NED Academy Course Banner

Use when the user wants a promotional banner or flyer for a new NED Academy course, workshop, or training, in the same layout as the "ChatGPT for Effective Learning" banner (portrait, A4-like).

## 1. Collect details with multiple-choice forms (AskUserQuestion)

All missing information must be collected through the AskUserQuestion form, not as a typed list of questions in chat. The form allows 1-4 questions per call and 2-4 options per question; the user can always pick "Other" to type a custom answer. Skip any question the user already answered in their request. Put the recommended option first and mark it "(Recommended)". Ask in the three rounds below, one AskUserQuestion call per round.

### Round 1: Course basics
- **Duration** (header "Duration"): 1-Day / 2-Day / 3-Day / 5-Day (Other for custom).
- **Mode** (header "Mode"): ONLINE / On-campus / Hybrid.
- **Audience** (header "Audience"): Teachers & Researchers / Students / Professionals & Engineers / Everyone (Other for custom).
- **Time slot** (header "Timings"): 2:00 pm to 4:30 pm / 10:00 am to 1:00 pm / 6:00 pm to 8:30 pm (Other for custom).

### Round 2: Schedule, fee, people
- **Days and start date** (header "Dates"): offer 2-3 concrete options computed from today's date (get it with the current-time tool), such as next Tuesday & Thursday, next Saturday & Sunday, or the following week (Other for custom).
- **Fee** (header "Investment"): Free / Rs. 1,000 / Rs. 1,500 / Rs. 2,500 per participant (Other for custom).
- **Facilitator** (header "Facilitator"): the user themselves, using the name, designation, and department known from the conversation or profile / Other (type name, designation, department). Do not invent one.
- **Modules** (header "Modules"): Draft them for me (5-6 modules with hours and bullets) / I will provide my own list.

### Round 3: Link, logos, theme, output
- **Registration link** (header "Join link"): I will paste the link now (Other) / Use a placeholder for now / Use a Google Meet link I already have in the chat.
- **Logos** (header "Logos"): Already attached / I will attach them next / Use text placeholders for now.
- **Theme** (header "Theme"): AI & technology / Engineering / Energy & petroleum / Education (Other for custom).
- **Output** (header "Output"): Editable design + PDF/PNG (Recommended) / PDF and PNG only / Also add a square social-media version.

If the user chooses "I will provide my own list" for modules, or "I will paste the link now", ask for that text in a short plain follow-up message, since it cannot be a multiple-choice answer. If the course title is not stated, propose one title in Round 1 by replacing the weakest question or ask in the same plain follow-up.

Do not invent facilitators, fees, dates, or links. Anything still unknown becomes a clearly visible placeholder on the banner.

## 2. Fixed elements (reuse for every course)

- Logos: NED University, CCEE, and NED Academy. Use the official logo files the user supplies exactly as given; never redraw or approximate the logos.
- Footer contacts: nedacademy@neduet.edu.pk; +92-21-99261261-8 Ext: 2297, 2397; http://academy.neduet.edu.pk; +92-314-2004528; social handles /neduet.academy, /neduet, @ned_academy. Confirm with the user if these have changed.

## 3. Layout (top to bottom)

1. **Header band (white):** NED University of Engineering & Technology logo left; CCEE and NED Academy logos right.
2. **Announcement strip (dark navy):** "NED Academy is offering [duration] [MODE] course", with the mode word highlighted in gold.
3. **Hero area:** themed photo/graphic background in navy tone. Large course title in white and gold, bold sans-serif. Audience line below in italic bold. On the right: schedule block (Timings, Commencement, Investment) with a small theme graphic beside it, and a "SCAN ME" QR code.
4. **Modules section:** two columns of numbered modules (I, II, III... in Roman numerals). Each has a bold heading with duration in brackets, then 2-3 short bullets. Balance the two columns.
5. **Join bar:** "Join Live Online Class" with the link in a highlighted strip at bottom-left.
6. **Facilitator box:** bottom-right, labeled FACILITATOR, with name, designation, and department.
7. **Footer (dark navy):** email, phones, website, and social handles with small icons.

## 4. Style

- Palette: deep navy (#0B1F4B-ish) background, gold (#F5B800-ish) accents for title and highlights, white text on dark, dark text on light panels.
- Fonts: bold sans-serif for titles, clean sans-serif for body, readable when printed.
- Bullets under about 12 words. Everything must fit one page without crowding.
- Generate the QR code from the supplied link with a script (for example Python qrcode); never draw it by hand.

## 5. Build and deliver

- If the session lists a Design artifact type, create the banner from it so the user can edit it. Otherwise build an HTML page and export to PDF and PNG (A4 portrait), using the pdf skill if needed.
- If the user asks for Word or PowerPoint, use the matching skill.
- Deliver the files with a one-line summary of what was filled in and which fields are still placeholders.

## 6. Check before finishing

- Dates, days, times, and fee match the form answers; day names match the dates.
- Module hours add up to the total course duration.
- QR code scans to the correct link.
- No spelling errors in names and designations.