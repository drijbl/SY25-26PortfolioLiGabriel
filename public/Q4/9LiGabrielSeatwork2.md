**Guided Question**: What changed compared to the default static positioning? Try to give different values to top and left or you can change it to bottom, right.

> When the sidebar was positioned static, it was laid out following the normal flow of the webpage, 
with no special positioning. However, when the sidebar was changed to position: absolute, it was removed from the 
normal flow of the document, and it was positioned relative to the element nearest to it by a distance that we specified to be 20px top and left. Changing
the values to top and left or changing it to bottom and right changed the distances for this relative positioning.

**Guided Question**: What happens when you scroll the page? Why does the footer behave differently from position relative?

> When you scroll the page, the footer remains at the bottom of the page, with the rest of the page and the elements moving with the footer above them. This happens because position: fixed specifies the footer to be independent to the scrolling body of the page.

**Guided Question**: What is the effect of position: absolute on an element? How is it different from fixed?

> Position: absolute relative to the initial containing block, with specified top, right, bottom, and left distances used for positioning it relative to this block. 
Compared to position: fixed, which positions the element in the same place regardless of scrolling, position: absolute allows the element to move with the scrolling.

**Guided Question**: Why does the notice appear on top of the content? What happens if you swap the z‑index values?

> The z-index in CSS basically determines the "priority level" of an object when it comes to stacking elements, with HTML elements with higher z-index values appearing above those with lower values. In this case, the notice appears on top of the content because it has a higher z-index value. If we were to swap these values, the notice would appear below the content instead.

## Reflection Questions
**a. Could you summarize the differences between the CSS position values (static, relative, absolute, fixed)?**
- Static: Positions an element according to the default positioning, appearing in the normal document flow.
- Relative: Positions an element relative to its normal position.
- Absolute: Positions an element relative to its nearest positioned ancestor.
- Fixed: Positions an element relative to the viewport, staying in place while scrolling. 

**b. How does absolute positioning depend on its parent element?**

Absolute positioning depends on its parent element by being positioning an element by the specified distance relative to the parent element.

**c. How do you differentiate sticky from fixed?**

Both sticky and fixed allow elements to remain visible during scrolling. However, a sticky elements acts like relative until it reaches a defined offset, then it it sticks in place within its parent container, going with this parent when it scrolls out of view. On the other hand, a fixed element is anchored to the view port, staying in the same place regardless of scrolling.

**d. If you were designing a webpage for a school event, how might you use positioning to highlight important information? Please give concrete examples.**

CSS Positioning allows for certain information to retain its position regardless of scrolling (e.g. fixed), while also allowing for some information to be positioned relative to the viewport or other elements. This could be used to arrange the information for the school event in a way that bests organizes it for clarity, readability, and function as an information provider for the details of the event. For example, if there are important information or widgets that need to be retained, such as the title of the event or navigation buttons that are important, fixed positioning could be used to keep it on the screen regardless of scrolling. On the other hand, you could use positioning to arrange information that doesn't have to be locked in the screen. Unimportant information could be positioned to the right sides or the bottom, where users don't typically start reading, to highlight this unimportance. Positioning also allows information to be organized such that the info is properly segmented, where you could position elements relative to each other to make the information organized rather than all vertically in the document. 

