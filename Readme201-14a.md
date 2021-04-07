# Transform Syntax

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.

Notice how the transform property includes multiple vendor prefixes to gain the best support across all browsers. The un-prefixed declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property.

In the interest of brevity, the remainder of this lesson will not include vendor prefixes. They are, however, strongly encouraged for any code in a production environment. Over time we will be able to remove these prefixes, however keeping them in is the safest approach for the time being.

1. 2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.

HTML CODE

(<div class="original"
  <div class="spin"
    <figure class="box box-1">Box 1</figure
  </div
</div

<div class="original"
  <div class="spin"
    <figure class="box box-2">Box 2</figure
  </div
</div)

CSS CODE 

body {
  color: #fff;
  font: 600 14px/24px "Open Sans", "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", Sans-Serif;
  margin: 12px 15px;
}
.original,
.box {
  border-radius: 6px;
}
.original {
  background: #eaeaed;
  border: 1px dashed #cecfd5;
  float: left;
  margin: 12px 15px;
}
.box {
  background: #2db34a;
  height: 95px;
  line-height: 95px;
  text-align: center;
  width: 95px;
}
.spin {
  cursor: pointer;
  transform-style: preserve-3d;
}
.spin:hover {
    animation: spin 5s linear infinite;
}
@keyframes spin {
  0% {
    transform: rotateY(0deg);
  }
  100% {
    transform: rotateY(360deg);
  }
}
.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

The gray box behind the rotated element symbolizes the original position of the element. Additionally, upon hover the box will rotate 360 degrees horizontally.

2. 2D Scale

Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

<div class="original"
  <div class="spin"
    <figure class="box box-1">Box 1</figure
  </div
</div

<div class="original"
  <div class="spin"
    <figure class="box box-2">Box 2</figure
  </div
</div

body {
  color: #fff;
  font: 600 14px/24px "Open Sans", "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", Sans-Serif;
  margin: 12px 15px;
}
.original,
.box {
  border-radius: 6px;
}
.original {
  background: #eaeaed;
  border: 1px dashed #cecfd5;
  float: left;
  margin: 12px 15px;
}
.box {
  background: #2db34a;
  height: 95px;
  line-height: 95px;
  text-align: center;
  width: 95px;
}
.spin {
  cursor: pointer;
  transform-style: preserve-3d;
}
.spin:hover {
    animation: spin 5s linear infinite;
}
@keyframes spin {
  0% {
    transform: rotateY(0deg);
  }
  100% {
    transform: rotateY(360deg);
  }
}
.box-1 {
  transform: scale(.75);
}
.box-2 {
  transform: scale(1.25);
}

It is possible to scale only the height or width of an element using the scaleX and scaleY values. The scaleX value will scale the width of an element while the scaleY value will scale the height of an element.

3. 2D Translate

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

<div class="original"
  <div class="spin"
    <figure class="box box-1">Box 1</figure
  </div
</div

<div class="original"
  <div class="spin"
    <figure class="box box-2">Box 2</figure
  </div
</div

<div class="original"
  <div class="spin"
    <figure class="box box-3">Box 3</figure
  </div
</div

body {
  color: #fff;
  font: 600 14px/24px "Open Sans", "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", Sans-Serif;
  margin: 12px 15px;
}
.original,
.box {
  border-radius: 6px;
}
.original {
  background: #eaeaed;
  border: 1px dashed #cecfd5;
  float: left;
  margin: 12px 15px;
}
.box {
  background: #2db34a;
  height: 95px;
  line-height: 95px;
  text-align: center;
  width: 95px;
}
.spin {
  cursor: pointer;
  transform-style: preserve-3d;
}
.spin:hover {
    animation: spin 5s linear infinite;
}
@keyframes spin {
  0% {
    transform: rotateY(0deg);
  }
  100% {
    transform: rotateY(360deg);
  }
}
.box-1 {
  transform: translateX(-10px);
}
.box-2 {
  transform: translateY(25%);
}
.box-3 {
  transform: translate(-10px, 25%);
}