# Guide Questions
## 1. STATIC vs RELATIVE — What changed compared to the default static positioning? Try to give different values to top and left or you can change it to bottom, right.
Compared to the static position, you can see it moved diagonally down and right. This is because it moved 20 pixels AWAY from the top and left. This means that the values you input indicates the distance from its static position.
## 2. FIXED — What happens when you scroll the page? Why does the footer behave differently from position relative?
When you scroll the page, it does not move from its position at all. Instead of positioning relative to its static position, "position: fixed;" means that the element will be anchored onto that place in the viewport. "bottom: 0;" and "width: 100%" simply means that it will occupy the entire bottom width.
## ABSOLUTE — What is the effect of position: absolute on an element? How is it different from fixed?
Unlike fixed positioning, which places the element relative to the viewport, absolute positioning places the element relative to its parent container.
## Z-INDEX — Why does the notice appear on top of the content? What happens if you swap the z‑index values?
The notice appears on top of the content because, while the latter has a z-index of 1, .notice has a z-index of 2. In CSS and HTML, an element with a greater z-index than another will always appear over that element. Any element with a z-index greater than zero will always appear over those without an indicated z-index, as 0 is the default.
---
# Challenge
## Try to change the position of .content to relative then to fixed. What do you observed each time?
It moves down 66 pixels when I change the position of .content to relative. Then, when I change it back to fixed, it returns to its original position.
## What do you observe on about the effect of z-index on .notice and .content boxes?
It gives .notice and .content a "priority" within the webpage for viewing, positioning it "above" (screen-wise, not in the webpage) other elements.
---
# Reflection
## a. Could you summarize the differences between the CSS position values (static, relative, absolute, fixed)?
Static is the default, relative positions the element relative to its static position, absolute positions the element relative to its parent, and fixed positions the element relative to the viewport.
## b. How does absolute positioning depend on its parent element?
Absolute positioning depends on its parent element in that it uses the latter as a reference point for its position.
## c. How do you differentiate sticky from fixed (you can research on sticky)?
While fixed positioning is anchored to the viewport, sticky is different in that it behaves like an element with "position: relative;" by moving along with the other elements. It only behaves like a fixed element when its "relative" position is not visible within the viewport anymore. If an object has, for example, "top: 100px;" and "left: 20px;", the object will stay in the viewport 100 px and 20 px away from the top and left side of the screen respectively.
## d. If you were designing a webpage for a school event, how might you use positioning to highlight important information? Please give concrete examples.
I would use fixed positioning on the navigation bar and footer to make them accessible anywhere in the page. As for position: absolute, I would use it for any element with a parent container, as it would make it easier to position. Relative positioning is also easier to use than static when it comes to fine-tuning the element's position; additionally, it would make absolute positioned elements easier to manipulate.