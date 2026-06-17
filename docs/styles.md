# CSS Style System

The style layer should use a small set of reusable CSS tokens for color, spacing, typography, borders, and focus states. Start with root variables such as `--color-text`, `--color-muted`, `--color-surface`, `--color-accent`, `--space-2`, `--space-4`, and `--radius-sm`. Components can then reference tokens instead of hard-coded values, which makes future theme changes safer and keeps visual rhythm consistent across landing pages, guide pages, and comparison sections.

```css
:root {
  --color-text: #172033;
  --color-muted: #5d6778;
  --color-surface: #ffffff;
  --color-accent: #0b6bcb;
  --space-4: 1rem;
  --radius-sm: 6px;
}

.guide-card {
  background: var(--color-surface);
  border: 1px solid #d8dee8;
  border-radius: var(--radius-sm);
  padding: var(--space-4);
}
```

Responsive rules should be content-led. Use fluid grids with `minmax()` for card lists, reserve fixed widths only for controls that need stable alignment, and keep readable line lengths on article pages. Focus outlines must remain visible for links, buttons, and accordion toggles. Avoid styling interactive elements only through color; combine color with underline, weight, border, or icon changes.

## Reference Resources

- [Safe Online Casino Philippines](https://casinosph.net/safe-online-casino-philippines/)
- [Bingo Plus Review](https://casinosph.net/bingo-plus-review/)
- [10 jili slot game register philippines](https://casinosph.net/10-jili-slot-game-register-philippines/)
- [arena plus apk latest version](https://casinosph.net/arena-plus-apk-latest-version/)
- [Best Online Casino Philippines](https://casinosph.net/)
- [Best Online Casino Philippines](https://casinosph.net/)
