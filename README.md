# Ezekiel39-koa.github.io
var xPositions = [250,300,150,50];
var yPositions = [0,100,200,300];
var leftX = 140;

draw = function() {
    background(204, 247, 255);
    
  
    for (var i = 0; i < xPositions.length; i++){
        noStroke();
        fill(0, 200, 255);
        if (yPositions[i] > 400){ 
            yPositions[i] = 0;
        }
            ellipse(xPositions[i], yPositions[i], 10, 10);
        yPositions[i] += random(1,10);
          var leftX = 140;
var rightX = 278;

     leftX +=-1;
     rightX +=1;
    // clouds 
    fill(189, 185, 189);
    // left cloud
    ellipse(leftX-38, 42, 126, 97);
    ellipse(leftX+40, 42, 70, 60);
    ellipse(leftX-111, 42, 70, 60);
    
    // right cloud
    ellipse(rightX, 94, 126, 97);
    ellipse(rightX+69, 94, 70, 60);
    ellipse(rightX-81, 94, 70, 60);
 // left cloud 2.
    ellipse(leftX-29, 120, 126, 97);
    ellipse(leftX+52, 120, 70, 60);
    ellipse(leftX-105, 120, 70, 60);
    
    // right cloud 2.
    ellipse(rightX, 40, 126, 97);
    ellipse(rightX+90, 40, 70, 60);
    ellipse(rightX-90, 40, 70, 60);
    
    }
   
};  
    var mouseClicked = function(){
    xPositions.push(random(0,400));
    yPositions.push(random(0,400));
};
