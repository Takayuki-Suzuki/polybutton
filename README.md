# polybutton
Swift class for creating polygonal buttons.

Create triangle, square, and other shape you can think of buttons in iOS.


![Sample_Buttons](https://github.com/benjaminhass/polybutton/blob/master/Screenshots/Sample_Poly_Buttons.png)

Usage:

Copy PolyButtons.swift into your project.
1. Create the vertices of the button.

var p1 = CGPoint(x: 200, y: 50.0)
var p2 = CGPoint(x: 300, y: 150.0)
var p3 = CGPoint(x: 100, y: 150.0)

2. Initialize with points, color, and bounds.

var triangle = PolyButton(points: [p1,p2,p3,], color: UIColor.greenColor(), frame: self.view.bounds)

3. Add an action, if desired.

func didPressTriangle(sender: AnyObject?) {
 println("Triangle")
}

triangle.action = didPressTriangle

4. Add the button as a subview to the parent view.
self.view.addSubview(triangle)
