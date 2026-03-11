# MCP Demo Site

A simple demo website created to test the **MCP Universal Command Center**.

## Structure

```
demo-site/
âââ index.html   â Main page with login button
âââ styles.css   â All styles (button position is here)
âââ README.md    â This file
```

## The Test

The **Login button** is currently positioned on the **RIGHT** side of the button area.

Use the MCP Command Center to move it to the right by giving this command:

> "Move the login button to the right and update the docs"

MCP will:
1. Scan this repo
2. Find the `.button-area` CSS rule in `styles.css`
3. Draft a change: `justify-content: flex-start` â’ `justify-content: flex-end`
4. Open a Pull Request
5. Update this README

## Current Button State

| Property | Current Value | Expected After MCP 
| --- | --- | --- |
| text-align | right | right |

Note: The styles.css file has been updated to reflect the new button position.
```css
/* styles.css */
.button-area {
  /* existing styles */
  text-align: right; /* Move login button to right side */
}
```