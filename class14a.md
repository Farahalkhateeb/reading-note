
# transform 
The transform CSS property lets you rotate, scale, skew, or translate an element. It modifies the coordinate space of the CSS visual formatting model.

# 2d skew 


2D Skew
The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis. To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.



# transform origin

The transform origin is the point around which a transformation is applied. For example, the transform origin of the rotate() function is the center of rotation.

In effect, this property wraps a pair of translations around the element's other transformations. The first translation moves the transform origin to the true origin at (0,0). Then the other transformations are applied, and because the transform origin is at (0,0), those transformations act about the transform origin. Finally, the opposite translation is applied, moving the transform origin back to its original location. Consequently, this definition


# Using CSS transitions
CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time. For example, if you change the color of an element from white to black, usually the change is instantaneous. With CSS transitions enabled, changes occur at time intervals that follow an acceleration curve, all of which can be customized.

Animations that involve transitioning between two states are often called implicit transitions as the states in between the start and final states are implicitly defined by the browser.

