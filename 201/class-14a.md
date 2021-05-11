# **Transforms**
The transform property comes in two different settings, two-dimensional and three-dimensional. 
**Syntax**
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

**2D Transforms**
work on the x and y axes.
1. the rotate value provides the ability to rotate an element from 0 to 360 degrees.
2. scale value allows you to change the appeared size of an element.
3. translate value works a bit like that of relative positioning.
4.  skew, is used to distort elements on the horizontal axis, vertical axis, or both.

![transforms](https://www.htmldog.com/figures/transform.png)

**3D Transforms**
work on both the x and y axes, as well as the z axis. we use here an new value rotateX, rotateY, and rotateZ.
**Transform Style**
To allow nested elements to transform in their own three-dimensional plane use the transform-style property with the preserve-3d value.

# **Transitions**
The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

![3d](https://miro.medium.com/max/900/1*_6MfwckxNfQTca9SiG8MdQ.png)

**properties**
1. transition-property
2. transition-duration
3. transition-timing-function
4. transition-delay

# **Animations Keyframes**
To set multiple points at which an element should undergo a transition, use the @keyframes rule. 

The vendor prefixes for the @keyframes rule:
* @-moz-keyframes
* @-o-keyframes
* @-webkit-keyframes

![animation](https://www.litmus.com/wp-content/uploads/2020/04/a-simple-guide-to-understanding-css-animations-in-email.png)

# **SIMPLE CSS3 TRANSITIONS**
1. Fade in: using opacity.
2. Change color using :hover and setting a new color.
3. Grow & Shrink using scale
4. Rotate elements using rotate
5. Square to circle using border-radius
6. 3D shadow 
7. Swing
8. Inset border



