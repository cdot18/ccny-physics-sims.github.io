---
title: motion 6
refno: eq-of-motion.6
width: 600
height: 100
---

<script>
var x0=0, x1=0, v0=0, a=.05, t=0, vel, accel;
function setup() {
  createCanvas(600,100);
  vel = 0;
  accel = .05;
}

function draw() {
  background(200);
  //method 1
  x = x0 + v0*t + 0.5* a * Math.pow(t,2);
  t+=1;
  fill('green');
  ellipse(x,height/1.5,10,10);
  //method 2
  x1 += vel;
  vel += accel;
  fill('red');
  ellipse(x1,height/2.5,10,10);
}
</script>
