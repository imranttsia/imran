---
name: "ned-academy-banner-redesign"
description: "Redevelop or refresh an existing NED Academy course banner or flyer; interview the user with multiple-choice forms to fill in every detail, then rebuild it."
---

# NED Academy Banner Redesign

Use when the user wants to redevelop, update, or restyle a course banner or flyer for NED Academy, either from an attached old banner or for a new course in the same family of layouts (portrait, A4-like, as in the "ChatGPT for Effective Learning" banner).

## 1. Read the source first

If the user attached a banner, read it before asking anything and extract: course title, duration, mode, audience, timings, dates, fee, modules with hours, join link, facilitator, and footer contacts. Treat these as known values and offer them as the first (recommended) option in the matching question. Never ask for something already visible in the attachment.

## 2. Interview with multiple-choice forms (AskUserQuestion)

Collect every missing detail through AskUserQuestion, not a typed list in chat. Each call takes 1-4 questions with 2-4 options each; the user can always choose "Other" to type a custom answer. Put the recommended option first and mark it "(Recommended)". Skip questions already answered. Use the four rounds below, one call per round.

### Round 1: What changes
- **Goal** (header "Goal"): Update dates/fee only / Fresh design, same content / New course, new content / Translate or adapt (Other for custom).
- **Course** (header "Course"): Keep the current title / Suggest 3 better titles for me / I will type a new title (Other).
- **Duration** (header "Duration"): 1-Day / 2-Day / 3-Day / 5-Day (Other for custom).
- **Mode** (header "Mode"): ONLINE / On-campus / Hybrid.

### Round 2: Audience and schedule
- **Audience** (header "Audience"): Teachers & Researchers / Students / Professionals & Engineers / Everyone (Other).
- **Timings** (header "Timings"): 2:00 pm to 4:30 pm / 10:00 am to 1:00 pm / 6:00 pm to 8:30 pm (Other).
- **Dates** (header "Dates"): offer 2-3 concrete options computed from today's date (use the current-time tool), such as next Tuesday & Thursday, next Saturday & Sunday, or the week after (Other).
- **Fee** (header "Investment"): Free / Rs. 1,000 / Rs. 1,500 / Rs. 2,500 per participant (Other).

### Round 3: Content and people
- **Modules** (header "Modules"): Keep the current modules / Draft new 5-6 modules for me / I will provide my own list.
- **Facilitator** (header "Facilitator"): Keep the current one / The user themselves, from known profile details / Other (type name, designation, department). Never invent a facilitator.
- **Registration link** (header "Join link"): Keep the current link / I will paste a new link (Other) / Placeholder for now.
- **Logos** (header "Logos"): Reuse from the attached banner / I will attach logo files next / Text placeholders for now.

### Round 4: Look and output
- **Style** (header "Style"): Same navy and gold look, cleaner spacing (Recommended) / Modern gradient with bold typography / Minimal light theme / Match a new theme (Other).
- **Theme graphic** (header "Graphic"): AI & technology / Engineering / Energy & petroleum / Education (Other).
- **Output** (header "Output"): Editable design + PDF/PNG (Recommended) / PDF and PNG only / Also a square social-media version.
- **Language** (header "Language"): English / English + Urdu headline / Urdu (Other).

If the user picks "I will provide my own list", "I will paste a new link", or "I will type a new title", ask for that text in one short plain follow-up, since it cannot be a multiple-choice answer.

Do not invent facilitators, fees, dates, or links. Anything still unknown becomes a clearly visible placeholder.

## 3. Fixed elements

- Logos: NED University, CCEE, NED Academy. Use the supplied or extracted logo files exactly; never redraw or approximate them.
- Footer contacts (confirm if unsure they are current): nedacademy@neduet.edu.pk; +92-21-99261261-8 Ext: 2297, 2397; http://academy.neduet.edu.pk; +92-314-2004528; social handles /neduet.academy, /neduet, @ned_academy.

## 4. Layout (top to bottom)

1. White header band with the three logos.
2. Navy announcement strip: "NED Academy is offering [duration] [MODE] course" with the mode word in gold.
3. Hero: themed navy-toned graphic, large course title, italic audience line, schedule block (Timings, Commencement, Investment), and a "SCAN ME" QR code.
4. Modules: two balanced columns, Roman-numeral headings with hours in brackets, 2-3 short bullets each.
5. "Join Live Online Class" bar with the link.
6. Facilitator box with name, designation, department.
7. Navy footer with email, phones, website, and social handles.

When the chosen style differs from the original, keep this information order and the fixed elements, and change only colors, typography, spacing, and imagery.

## 5. Build and deliver

- Generate the QR code from the supplied link with a script (for example Python qrcode); never draw it by hand.
- If the session lists a Design artifact type, create the banner from it so it stays editable. Otherwise build an HTML page and export PDF and PNG at A4 portrait.
- Use the docx or pptx skills only if the user asks for Word or PowerPoint.
- Deliver with a one-line summary of what changed from the original and which fields are still placeholders.

## 6. Check before finishing

- Dates, weekdays, times, and fee match the form answers.
- Module hours add up to the stated course duration.
- The QR code resolves to the correct link.
- Names, designations, and contact details are spelled correctly.
- Text fits on one page without crowding; bullets stay under about 12 words.