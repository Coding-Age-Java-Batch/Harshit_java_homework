    abstract class Game {
    void start(){
    System.out.println("Game started");
    }
    abstract void play();
    }
    class Cricket extends Game{
    void play(){
    System.out.println("Playing Cricket");
    }
    }
    class Chess extends Game{
    void play(){
    System.out.println("Playing chess");
    }

    static void main(String[] args) {
        Game ct = new Cricket();
        Game ch = new Chess();

        ct.start();
        ct.play();

        ch.start();
        ch.play();
    }
    }
