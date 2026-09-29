# Monsoon Trails: quotation customizer

A consumer-facing take on a travel agent's quotation. A customer opens the quote they received, changes a few things (hotels, activities, rooms), sees the price impact, reviews every change against the original, and sends the revised quotation back to the agent.

Built as a design-engineering exploration: requirements written by me, drafted with Claude Design, tested and critiqued by me, refined by hand in Figma, and the final decisions carried back into this HTML.

**Live demo:** _add your GitHub Pages link here_
**Figma:** _add link here_

## The flow

1. Open the quotation
2. Review the itinerary city by city
3. Customize hotels, rooms and activities
4. See price impact and the updated total
5. Compare the original with the revised quotation
6. Review and send to the agent

## Product decisions

- The agent stays in control: nothing is final until the agent confirms.
- Price states, not just prices: locked, needs agent confirmation, or included.
- Changes shown as a diff against the original quotation.
- Edge cases designed early: time clashes, split stays in one city, expired quotes.
- Scoped on purpose: no login, payments, real inventory, backend or chatbot.

## Run it locally

Serve the folder (some browsers block the scripts over `file://`):

```
python3 -m http.server
```

Then open http://localhost:8000

## Files

- `index.html`: the prototype (design component plus a small logic class)
- `assets/`: photography and images
- `vendor/`, `support.js`: the runtime that renders the component

## Tools

Claude Design for drafting, Figma for refinement and tokens, HTML for the final build.

Made by Kavya Shivastava.
