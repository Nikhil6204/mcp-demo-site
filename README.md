# MCP Demo Site

A simple demo website created to test the **MCP Universal Command Center**.

## Structure

```
demo-site/
├── index.html   ← Main page with login button
├── styles.css   ← All styles (button position is here)
├── README.md    ← This file
```

## The Test

The **Login button** is currently positioned on the **RIGHT** side of the button area.

Use the MCP Command Center to move it to the right by giving this command:

> "Move the login button to the right and update the docs"

MCP will:
1. Scan this repo
2. Find the `.button-area` CSS rule in `styles.css`
3. Draft a change: `justify-content: flex-start` → `justify-content: flex-end`
4. Open a Pull Request
5. Update this README

## Current Button State

| Property | Value |
| --- | --- |
| justify-content | flex-end |

Note: The styles.css file has been updated to reflect the change:
```css
/* styles.css */
.b {
  /* ... existing styles ... */
  justify-content: flex-end; /* Changed from flex-start to flex-end */
}
```