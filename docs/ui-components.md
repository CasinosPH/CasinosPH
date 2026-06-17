# UI Components Guide

The component layer should be built from small HTML patterns that can be reused without changing content structure. Core components include the site header, responsive navigation, article summary card, comparison table, status badge, FAQ accordion, and call-to-action group. Each component should accept plain data and render semantic HTML first, then apply CSS classes for layout and states. For example, a card should use an `article` element, a heading link, a short summary paragraph, and a footer area for metadata.

```html
<article class="guide-card">
  <h2><a href="/guides/sample/">Guide title</a></h2>
  <p>Short summary text for scanning.</p>
  <footer><span class="badge">Updated</span></footer>
</article>
```

Interactive components need clear keyboard behavior. The accordion should use a button for each question, keep `aria-expanded` synchronized with the open state, and preserve focus after toggling. Table components should remain readable on small screens by using horizontal overflow only when columns cannot collapse safely. Buttons should distinguish primary actions, secondary actions, and neutral text links through class names rather than inline styles.

Component markup should avoid decorative wrappers that add no meaning. The preferred approach is to expose predictable slots: title, body, media, action, and supporting note. This lets templates render article pages, bonus summaries, and guide indexes with the same surface while keeping the DOM easy to test.

## Reference Resources

- [Free Spins Philippines](https://casinosph.net/free-spins-philippines/)
- [Casino Welcome Bonus](https://casinosph.net/casino-welcome-bonus/)
- [GCash Casino Deposit](https://casinosph.net/gcash-casino-deposit/)
- [Maya Casino Withdrawal](https://casinosph.net/maya-casino-withdrawal/)
- [Best Online Casinos Philippines](https://casinosph.net/)
- [Best Online Casino Philippines](https://casinosph.net/)
