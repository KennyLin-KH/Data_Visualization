let dayno = 0;
let circleColor;
let circles = [[200,200,100],[400,200,100],[200,400,100],[400,400,100],[200,600,100],[400,600,100]];
let times = [[4,5,7,5,1,1],[4,5,7,5,1,1],[6,8,8,0,2,0],[5,7,7,0,0,3],[4,7,7,5,1,2],[4,6,7,5,1,1],[5,8,8,2,1,2],[6,7,7,5,1,1],[5,8,8,2,1,0],[3,9,9,0,2,0],[4,9,8,0,0,3],[5,8,7,3,1,2]];

function setup() {
  createCanvas(600, 800);
}

function draw() {
  if (dayno > 5) {
    dayno = 0;
  }
  background(200);
  for (x = 0; x < 6; x++){
    circolor = dataColors(times[dayno][x])
    if (x == 0){
      fill (circolor, 0,0);
    }
    else if (x == 1){
      fill (0, circolor, 0);
    }
    else if (x == 2){
      fill(0,0,circolor);
    }
    else if (x== 3) {
      fill(circolor,circolor,0);
    }
    else if (x == 4) {
      fill(circolor, 0, circolor);
    }
    else if (x == 5) {
      fill(0,circolor,circolor);
    }
    circle(circles[x][0],circles[x][1],circles[x][2])
  }
}

function dataColors(x) {
  x *= 22;
  return x;
}
function keyReleased() {
  dayno++
}
