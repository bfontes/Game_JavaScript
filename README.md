let x = 200;
let y = 350;
var colidiu=false;

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(20)
  
  if(keyIsDown(DOWN_ARROW)){
    if(y + 20 < 400){
      y = y + 3;}
  }
  
  if(keyIsDown(UP_ARROW)){
    if(y - 20 > 0){
    y= y - 3}
  }
  
  if(keyIsDown(RIGHT_ARROW)){
    if(x + 20 < 400){
    x= x + 3}
  }
  
  if(keyIsDown(LEFT_ARROW)){
    if(x - 20 > 0){
    x= x - 3}
  }
  
  ellipse(x, y, 40, 40);
  
  if(colidiu===true){
     x = 200;
    y = 350;
    colidiu=false
  }
   
    if(y + 20 < 400){
     // y = y + 3;
    }
  
  
  
    if(y - 20 > 0){
    //y= y - 3
    }
  
  

    if(x + 20 < 400){
   // x= x + 3
    }

  

    if(x - 20 <90){
      colidiu=true
    }
  
  
  square(30, 30, 60);

}
