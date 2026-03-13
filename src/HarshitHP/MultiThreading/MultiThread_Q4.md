public class A extends Thread {
public void run() {
try {
System.out.println("A Start");
Thread.sleep(1000);
System.out.println("A End");
} catch (InterruptedException e) {
System.out.println(e);
}
}

    static void main(String[] args) {
        A t1 = new A();

        try {
            t1.start();

            t1.join();
        } catch (InterruptedException e) {
            System.out.println(e);
        }
        System.out.println("Main After A");
    }
}
