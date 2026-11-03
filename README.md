# AI Syllabus Statements graphic

This is a one-page graphic that explains the four AI statements instructors can put in a WKU syllabus: **AI Prohibited, AI Planning, AI Refinement, and Full Use**. It shows them on a scale from most restrictive to most open, with what students may and must do under each. It was made by the WKU AI Committee's Student Subcommittee.

**Status:** the wording has not yet been approved by the AI Committee, the Provost, or the Office of Student Conduct. Please don't publish it until it has been.

## What's in this folder

| File | What it is | Who needs it |
| --- | --- | --- |
| `assets/ai-syllabus-statements.png` | The finished picture, 3200 pixels wide. | Anyone who wants to drop it in a slide, email, PDF, or print it. |
| `fragment.html` | The same graphic as web page code. | The web team, to put it on a page. |
| `css/ai-syllabus-statements.css` | The styling (colors, fonts, layout) for that code. | The web team. |
| `index.html` | A ready-made test page that shows the graphic on its own. | Anyone who wants to preview it in a browser. |

## If you just need the picture

Use `assets/ai-syllabus-statements.png`. Alt text for screen readers:

> AI Syllabus Statements. Four options from most restrictive to most open: 1 AI Prohibited, 2 AI Planning, 3 AI Refinement, 4 Full Use. Your instructor chooses one for the course or for each assignment. Check your syllabus to see which applies.

## If you're putting it on a web page (web team)

1. Add `css/ai-syllabus-statements.css` to the site, or copy its contents into the site's stylesheet.
2. Open `fragment.html`, copy everything in it, and paste it where the graphic should go.
3. If the page already has a main title, change the graphic's top heading from `h1` to `h2`, and move the smaller headings down one level to match.

It uses real text, not a picture, so it is readable by screen readers and resizes on phones. It needs no scripts and loads nothing from outside sites. On wku.edu the fonts load automatically from the site.

## Before it goes live

- [ ] Get the wording approved (see Status above).
- [ ] Ask Melanie Evans, who drafted the statements, to check the short summaries in the graphic. They are plain-language rewrites, not the exact syllabus text.
- [ ] Confirm the line "From the Provost's AI Committee / Student Subcommittee" in the header is right. It was carried over from the original infographic.
- [ ] Check the link at the bottom (libguides.wku.edu/stylewrite/ai).
- [ ] Decide whether the lighter red steps in the scale are acceptable (see Colors).

## Colors and fonts

The graphic uses WKU's web colors from the [WKU colors page](https://www.wku.edu/web-cms/best-practices/colors/): WKU Red `#B01E24`, WKU Red (Darker) `#9A1A20`, Text Gray `#555555`, Black Gray `#222222`, Lighter Gray `#CCCCCC`, and Lightest Gray `#EFEFEF`. The fonts match wku.edu: Open Sans for text and Overpass for headings.

One thing is outside that palette: the four steps of the scale are WKU Red fading toward white, so the steps can show "more open" visually. Those lighter reds are not WKU palette colors.

It does not use the WKU logo.

## Accessibility

All text and background pairs were checked and meet the WCAG AA contrast minimum (4.5 to 1 for normal text, 3 to 1 for large text). The meaning never depends on color alone, because every option is named and numbered. The scale bar and number circles are decorative and are hidden from screen readers.

## Changing the text or making a new picture (technical)

- To change the wording, edit `fragment.html` and re-copy it into `index.html`. Class names all start with `ai-statements` or `tier`, so the styles won't affect the rest of a site.
- To export a new PNG you need Google Chrome. Open a page that loads Open Sans and Overpass, then run Chrome in headless mode at 1600 pixels wide with `--force-device-scale-factor=2`, and crop to the graphic. Without those two fonts installed or loaded, the picture will fall back to Arial.
- The layout switches between four columns and one stacked column based on the width of the space it's placed in, not the screen. Very old browsers show the stacked version.
