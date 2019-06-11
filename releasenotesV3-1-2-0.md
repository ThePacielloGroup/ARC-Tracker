# June 2019 ARC Release Version 3.1.2.0
## Updates

- **Bug Fixed** I run my browser and dev tools in dark mode. The text in ARC is black on gray. The only table rows I can read are the gray zebra-striped rows.
- **Bug Fixed** The color contrast test is showing that insufficient contrast passes.
- **Bug Fixed** Duplicate id attribute values are not picked up by ARC rules, unless used with labels. Duplicate id attributes can cause problems when used in other programmatic combinations, such as aria-controls, aria-activedescendant, and so on.
- **Bug Fixed** an SVG image with an accessible name supplied using the aria-labelledby attribute is marked as an error
- **New Feature** [WCAG 2.1 1.3.5: Identify Input Purpose](https://w3c.github.io/wcag21/understanding/identify-input-purpose.html) test
