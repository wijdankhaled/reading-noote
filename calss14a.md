# Transforms
The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

**2D Transforms**
Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis.

- **2D Rotate**
The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees

![](https://blog.udemy.com/wp-content/uploads/2014/01/2Drotate.png)

 - 2D Scale

 Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and

- 2D Translate

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical ax

- 2D Skew
The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both. The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRyyTs4TaodGxBnIQqtuH7IeowD4uV6trHPAw&usqp=CAU)

**Combining Transforms**

It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together

**Transform Origin**
As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used

**Transitions & Animations**

**Animations**
Transitions do a great job of building out visual interactions from one state to another, and are perfect for these kinds of single state changes. However, when more control is required, transitions need to have multiple states
 
- Animation Name

Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value

![](https://assets.materialup.com/uploads/42ce3158-ac1d-42d6-9d6a-4c6b5f7e9507/preview.gif)

**Backface Visibility**

When working with three-dimensional transforms, elements will occasionally be transformed in a way that causes them to face away from the screen. This may be caused by setting the rotateY(180deg) value for example. By default these elements are shown from the back
