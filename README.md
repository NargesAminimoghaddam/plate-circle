# plate-circle
var x = 20;
var y = 20;
var xSpeed = 1;
var ySpeed = 2.3;

draw = function() {
    background(26, 161, 35);
    
    fill(sin(2*x)*10, cos(2*x)*10, sin(x)*10);
    ellipse(100*sin(3*x)+100, 100*cos(3*x)+100, 50, 50);

 
    x = x + xSpeed;
    y = y + ySpeed;
    
    // Check for bouncing.
    if ((x > width)  (x < 10)) {
        xSpeed = xSpeed * -1;
    }
    if ((y > height)  (y <10)) {
        ySpeed = ySpeed * -1;
    }
    
    noStroke();
    fill(216, 230, 18);
  
    ellipse(x, y, 300, 30);
    
    
};
