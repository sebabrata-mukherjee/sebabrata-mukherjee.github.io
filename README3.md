// import library
import imageN.*;
// create a reference to an image sequence
ISPlayer player;

void setup() {
  size(640, 360);
  // create instance and load all valid images from the data folder
  player = new ISPlayer(this,dataPath("name-of-image-folder-in-data"));
}

void draw() {
  // clear background with yellow
  background(255, 204, 0);
  // render image sequence, ISPlayer extends PImage, use it as such
  image(player,mouseX,mouseY);
}

// image sequence events
// all frames loaded
void onSequenceLoaded(ISPlayer player){
  println(player+" sequence fully loaded");
  player.loop();
}
