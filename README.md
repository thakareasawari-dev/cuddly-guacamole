# cuddly-guacamole

"Tired of bloated software generating hundreds of kilobytes of code for simple inputs? I built an interactive terminal application using raw HTML, vanilla JS, and zero divs. It runs perfectly under 3 KB and renders instantly while modern stacks take a minute to process JSON files. Let me know what you think of the architecture."

---

## Files

### 📄 `index.html` - The Original
The main semantic HTML chaos page featuring:
- ✅ Interactive button that flips between dark/light mode
- ✅ Nested `<fieldset>` checkboxes for existential confirmation
- ✅ Progress bar that fills as you check boxes
- ✅ `<details>` section asking "do you know if I'm sure?"
- ✅ Confusing heading hierarchy (h1-h6)
- ✅ Accessibility table (TalkBack, VoiceOver, NVDA, etc.)
- ✅ Fruit lists (because why not?)
- ✅ When all checkboxes are checked → H1 changes to "CONGRATULATIONS. YOU WASTED 20 SECONDS."

Works perfectly with screen readers like TalkBack despite being intentionally absurd.

### 🔥 `hell.html` - The Rickroll Trap
Same as `index.html` BUT:
- 🎯 **The H1 heading is wrapped in a rickroll link**
- Users think it's semantic HTML chaos
- Click the heading → **Never gonna give you up** 🎵
- Announces as "Heading 1. Link." on screen readers
- Valid HTML. Perfectly accessible. Completely trolling.

---

## How It Works

**The Checkbox Logic:**
```javascript
Check all 3 nested checkboxes → Progress bar fills to 100% → H1 text changes
```

**The Button:**
```javascript
Click "click me." → Dark mode ↔ Light mode (100% brightness flip)
```

**The Rickroll (hell.html only):**
```html
<h1>
    <a href="https://youtu.be/dQw4w9WgXcQ">
        do you think that this is a link?
    </a>
</h1>
```

---

## TalkBack Announcements

When using TalkBack (Android screen reader):
- "Heading 1" (or "Heading 1. Link." if viewing `hell.html`)
- "Collapsed. Click here to see if I'm sure. Disclosure triangle"
- "Heading that stands in the middle of the road"
- All semantic structure announced perfectly despite the chaos

---

## The Point

Built with:
- Raw HTML (semantic structure)
- Vanilla JavaScript (no frameworks)
- CSS (minimal styling)
- **Zero divs** (uses `<fieldset>`, `<details>`, `<table>`, proper heading hierarchy)

This demonstrates that you don't need bloated frameworks to build interactive, accessible web experiences. 

Also, rickrolls are funny. 🎭
