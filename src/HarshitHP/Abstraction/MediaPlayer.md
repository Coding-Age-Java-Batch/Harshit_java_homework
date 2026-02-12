abstract class MediaPlayer {

    protected String filename;

    MediaPlayer(String filename){
        this.filename = filename;
    }
    abstract void play();
}
class AudioPlayer extends MediaPlayer{
AudioPlayer(String filename){
super(filename);
}
void play(){
System.out.println("Playing audio: "+ filename);
}
}
class VideoPlayer extends MediaPlayer{
VideoPlayer(String filename){
super(filename);
}
void play(){
System.out.println("Playing video: "+filename);
}

    static void main(String[] args) {
        MediaPlayer audio = new AudioPlayer("song.mp3");
        MediaPlayer video = new VideoPlayer("movie.mp4");

        audio.play();
        video.play();
    }
}
