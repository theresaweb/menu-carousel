This is a work in progress, an attempt to make a cleanly coded flexbox/javaScript carousel to be used with varying width menu items.

   # Requirement:
* An unordered list should be displayed horizontally within a responsive width
* The items in the unordered list are of varying widths
* the "next" group of items should include and partially visible items in the "current" view
* When the first item in the unordered list is visible it should be flush against the left side of the box and the left arrow should not be visible
* When the last item in the unordered list is visible, the right arrow should not be visible ?? should it?
* When the last item in the unordered list is visible,  it should be flush against the right side of the box
* The unordered list should maintain it's position when the box resizes ??

   # Method:
1. Calculate width of each item and width of box, build a list of sections and show accordingly
2. Calculate the width of the most items that can be fully visible and move the slider right and left that much,
adjust first and last section to be flush against the side

    # Consider Performance:
* https://www.sitepoint.com/10-ways-minimize-reflows-improve-performance/
* https://developer.mozilla.org/en-US/docs/Web/API/CSS_Object_Model/Determining_the_dimensions_of_elements
