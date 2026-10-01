<!--
This file provides context/instruction for your repository! They are written in Markdown (.md), for simple formatting:
https://www.markdownguide.org/cheat-sheet/
-->

# Project 1: Hooked On A Feeling Manuscript

A response to Michael Rock’s *Hooked on a Feeling* (2015), typeset as a single web page.[LIVE SITE](https://simrinrajani.github.io/manuscript/).

>## The reading
>Rock argues that design has always moved between function and feeling, and that the balance is shifting more towards feeling.
>## My response
>I agree with Rock, and I push his argument further: function and feeling aren’t opposites. Feeling is part of whether a functional solution actually works. Reading the article again in 2026, with AI optimizing for speed and efficiency, I think designing feeling matters even more.

>## Design concept
>The page is a conversation, not a debate. Rock’s text flows into mine.
**Rock’s article sits on light paper, and my response sits on near-black.**
A gradient blends one into the other instead of a hard cut, because I’m continuing his argument, not opposing it.
**“ROCK:” is hollow and “ME:” is solid.**
His article is the framework, and my response fills it in.
**The quotes stay neutral, and only the words carry color.**
That way you can see function and feeling living inside the same sentence.

>## The system
**Color: each color used intentionally**
- Coral = feeling
- Teal = function
- Hot pink = interaction (anything you can click)
- Gold = the reader’s highlighter
**Type: one job per font**
- Archivo: strong claims (headlines, big statements)
- DM Serif Display: feeling and quoted ideas
- Source Serif 4: long reading
- IBM Plex Mono: data and interface (labels, nav, credits)
**Semantic tags carry the color system**
- `<i>` is defined as “an alternate voice or mood,” so it marks feeling words (coral).
- `<b>` is for “utilitarian” attention, so it marks function words (teal).
- `<em>` original meaning=stress emphasis.
**Interaction**
- Hovering reveals feeling/glow
- Hovering each closing question reveals whether it’s function or feeling

>## How I made it

- HTML and CSS only: no images, no flex or grid.
- Created a desiign system of sizes, spacing, fonts and colors are CSS variables in `:root`, in `rem`, from a single root size.
- Styles go from general to specific: global tags first, then each section, then classes and pseudo-classes.
- Course name and date top line bar sit on opposite edges using `text-align: justify`, a typesetting technique, instead of a layout tool.
FYI: used claude and chat to ask questions when I needed an explaination for something to help understand errors and fix them, also asked for periodic critiques to get the most out of my work


## Things I want to remember

- `blockquote.feeling` (no space) means a blockquote *with* the class. `blockquote .feeling` (with a space) means something *inside* a blockquote- broke my layout a few times until I figured out the issue
- Renaming a variable silently breaks every rule still using the old name (I made quite a few color changes along the way to hit a sweet spot and every time I changes them I had to make sure they were updated everywhere in the page)
- Margin is outside the box and padding is inside, so backgrounds only fill padding (black background section- used padding instead of margin for full bleed)
- `text-align-last: justify` is what makes justify work on a single line, that was was hard to figure out
