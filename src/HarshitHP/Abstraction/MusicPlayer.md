    interface MusicPlayer {
     void playSong(String name);
    }
    class  SpotifyPlayer implements MusicPlayer{
     public void playSong(String name){
     System.out.println("Playing song on Spotify: " +name);
     }
     public void pause(){
     System.out.println("Spotify playback paused");
     }
    }
    class LocalPlayer implements MusicPlayer{
     public void playSong(String name){
     System.out.println("Playing local song: " +name );
      }
     public void pause(){
     System.out.println("Local music paused");
      }

    static void main(String[] args) {
        SpotifyPlayer sp = new SpotifyPlayer();
        LocalPlayer lp = new LocalPlayer();

        sp.playSong("Kesariya");
        sp.pause();

        lp.playSong("Teri Mitti");
        lp.pause();
     }
    }