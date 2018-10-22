# Remove-ouline-click-only
Test different solution about remove outline styling just click event only

## 1. [:focus-visible](https://drafts.csswg.org/selectors-4/#the-focus-visible-pseudo)

## 2. [What-input](https://github.com/ten1seven/what-input)

## 3. [Smart-outline](https://github.com/ambassify/smart-outline)

There are 4 different solution to tracking the input method(mouse keyboard)

**1. what-input**
https://github.com/ten1seven/what-input

**2. smart-outline**
(https://github.com/ambassify/smart-outline)

**3. :focus-visible**
https://drafts.csswg.org/selectors-4/#the-focus-visible-pseudo
https://github.com/WICG/focus-visible


**4. use tabindex and customise label included at interactive element**


for example


instead of:
```
<button id="btn" class="btn" type="button">I'm a button!</button>
```

do this:

```
<button id="btn" class="btn" type="button">
    <span class="btn__content" tabindex="-1">
        I'm a button!
    </span>
</button>
```

I also write some demo to test each one,I found the **what-input** works well in different browser(Chrome Firefox IE Safari ), so I propose we can use what-input to distinguish the keyboard and mouse event.

