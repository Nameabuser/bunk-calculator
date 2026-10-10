# Bunk Calculator

**Skip smart, not blind.** Type in how many classes you attended and how many have happened. It tells you how many you can still bunk, or how many you must attend in a row to get back above the line.

**Live:** https://nameabuser.github.io/bunk-calculator/

![Bunk Calculator on a phone](screenshot.png)

## What it does

- Enter classes attended, total classes so far, and the attendance % your college needs (75% by default).
- Above the line: shows how many classes you can skip and still stay at or above the requirement.
- Below the line: shows how many classes in a row you have to attend to recover.
- Save subjects, then tap "Attended today" or "Bunked today" to update the count.
- Works on any phone or laptop browser. Add it to your home screen if you like.

## The maths

With `a` attended, `t` total and required `r` percent:

- Safe bunks = floor(a x 100 / r - t)
- Classes to attend to recover = ceil((r x t - 100 x a) / (100 - r))

## Privacy

No sign-up, no server, no tracking. Your numbers are saved only in your own browser (localStorage).

## Limits

It does a simple attendance percentage. It does not know your college's special rules such as medical leave, condonation, or rounding. Check your own rules before you bunk for real.

## Run it yourself

It is a single `index.html` file. Open it in a browser, or host it on GitHub Pages.
