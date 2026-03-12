public class MyThreadExmp extends Thread{

    public void run(){
        System.out.println("Hello from MyThread");
    }

    static void main(String[] args) {
        MyThreadExmp mt = new MyThreadExmp();
        mt.start();
    }
}