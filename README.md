<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>Pietro Piga - Processign Project</title>
        <script src="vendors/processing.min.js"></script>
    </head>
    <body>
        <h1>Processing project by Pietro Piga </h1>
        <script type="text/processing">
void setup () {
  size (400, 400);
  background (255);
  smooth ();
  noStroke ();
  frameRate (200);
}
void draw () {
  
  fill (frameCount * 50 % 255, frameCount * 100 % 255, frameCount * 150 % 255, frameCount * 200 % 255);
  pushMatrix ();
  translate (200, 200);
  rotate (radians (frameCount * 70 % 360));
  ellipse (150, 100, 80, 30);
  popMatrix ();
}
