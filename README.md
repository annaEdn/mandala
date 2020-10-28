# mandala

int i = 0;
int a = 250;
int b = 0;

void setup() {
   
   background(150);
   
   size(screenWidth, screenHeight);
   rectMode(CENTER);
   }
 void draw() {		
	
   pushMatrix();
      	translate(width/2, height/2);
      	rotate(radians(2*-i));
      
       	noFill();
         rect(100,0,500,500);
			popMatrix();

		pushMatrix();
      translate(width/2, height/2);
      rotate(radians(2*i));
      
      if (b<250, i<500){
         fill(a,0,b,10);
         rect(200,0,100,100);
         i+=2;
         a-=2;
         b+=2;
     
      }else {			
         fill(b,0,a,10);
         rect(200,0,100,100);
				i+=2         
				a+=2
          b-=2;   	
		
		popMatrix();

		pushMatrix();
      	translate(width/2, height/2);
      	rotate(radians(i));
      	i+=10
       	noFill();
         ellipse(100,0,100,100);
			popMatrix();

		
		pushMatrix();
      translate(width/2, height/2);
      rotate(radians(0.3*-i));
      
      if (b<250, i<500){
         fill(a,0,b,10);
         rect(40,0,60,60);
         i+=2;
         a-=1;
         b+=1;
         
      }else {			
         fill(b,0,a,10);
         rect(40,0,60,60);
				i==0         
				a+=1
         b-=1;   	
		}
		popMatrix()


      pushMatrix();
      translate(width/2, height/2);
      rotate(radians(0.1*i));
      
       noFill();
         ellipse(40,0,300,300);
			popMatrix();
 		

   
   }
   
}
   
      

