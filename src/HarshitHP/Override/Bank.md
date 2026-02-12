    class Bank {
    int getIntresetRate(){
     return 0;
     }
    }
    class SBI extends Bank{
    @Override
    int getIntresetRate(){
     return 5;
     }
    }
    class HDFC extends Bank{
    @Override
    int getIntresetRate() {
     return 6;
     }
    }
    class ICICI extends Bank{
    @Override
    int getIntresetRate() {
     return 7;
     }

    static void main(String[] args) {
        Bank sbi = new SBI();
        Bank hdfc = new HDFC();
        Bank icici = new ICICI();

        System.out.println("SBI Intreset Rate: " +sbi.getIntresetRate()+ "%");
        System.out.println("HDFC Intreset Rate: " +hdfc.getIntresetRate()+ "%");
        System.out.println("ICICI Intreset Rate: " +icici.getIntresetRate()+ "%");
     }
    }