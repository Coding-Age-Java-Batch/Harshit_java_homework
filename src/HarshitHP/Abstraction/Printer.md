    interface Printer {
    void print(String document);
    }
    class InkjetPrinter implements Printer{
    public void print(String document){
    System.out.println("Inkjet printer printing document: " +document);
    }
    }
    class LaserPrinter implements Printer{
    public void print(String document){
    System.out.println("Laser printer printing: " +document);
    }

    static void main(String[] args) {
        Printer ip = new InkjetPrinter();
        Printer lp = new LaserPrinter();

        ip.print("Resume.pdf");
        lp.print("Report.pdf");
    }
    }