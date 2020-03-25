## 과제 2-2 한글 위 아래로 움직이게 하기 ##

PFont f;

void setup(){

size(800,300);

f = createFont("굴림",64);

textFont(f);

}

int i, dir=1,sp=1;

void draw() {

fill(0);

 background(0,255,0
 
 text("안동대 컴공 사랑합니다♥", 50, i);
 
 if(i>width-128/2*7) dir=-1;
 
 if(i<0) dir=1;
 
 i = i+dir*sp;
 
  //if (keyPressed) sp = key-'0';
  
}

void keyPressed(){

  sp = key -'0';
  
}

