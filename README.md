# auto-ufo-spel

```
//beweeg auto 1/variabele = een plekje in het geheugen met een naam//
float X = 0;

 //De y coordinaat van de auto//
float dY = 0.1; 
//De verandering van de y coordinaat van de auto//
float Y = 0; 
 


 
void setup(){

 
  //scherm// 
  size(700,500,P3D);
  
  


}
 

 
 
 void draw(){
 ellipse( X + 60,100,47,29);
   //achtergrond//
   background(155,98,118);
  stroke(255,255,0);
  fill(0,0,0);
  rect(0,0,700,300);
  //steren 1//
  point(350,75);
  point(350,70);
  point(350,80);
  point(350,65);
  point(350,85);
  point(350,60);
  point(350,90);
  point(350,95);
  point(350,100);
  //weg 1//
  fill(100,100,150);
  rect(0,370,700,100);
  stroke(255,255,255);
  line(165,335,200,335);
  line(340,335,375,335);
  line(515,335,550,335);
  line(25,335,50,335);
  line(640,335,685,335);
  //steren 2//
  stroke(255,255,0);
  point(60,120);
  point(610,200);
  point(490,81);
  point(399,277);
  point(64,222);
  point(655,11);
  point(322,544);
  //maan//
  fill(190,190,190);
  ellipse(200,50,200,150);
  //auto//
  fill(0,0,0);
  ellipse(X + 40,Y + 335,50,50);
  rect(X + 30,Y + 270,175,40);
  ellipse(X + 190,Y + 335,50,50);
  rect(X + 60,Y + 200,120,70);
  fill(0,190,200);
  rect(X + 140,Y + 220,30,35);
  rect(X + 80,Y + 220,30,35); 
  fill(255,255,0);
  //beweeg auto 2//
  X = X + 5;
  Y = Y + dY;
   if (X > 700)
  {
    X = -50;
  }
 //ufo//
 fill(0,255,0);
 ellipse(mouseX,mouseY,100,25);
 fill(100,100,100);
 ellipse(mouseX,mouseY,50,35);
 
 
 
   

 
 
 }
 

 
 
 
 
 

 
 void keyPressed() 
 {
  dY = -dY;
    if (X == 0)
    {
      X = 255; 
    }
   else 
   {
     X = 0;
   }
 }
 
 

```
