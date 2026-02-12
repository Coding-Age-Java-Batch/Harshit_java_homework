    class Student_1 {
    String Name;
    Student_1(String n){
    Name = n;
    }
    void display(){
    System.out.println("Name: " +Name);
    }
    }

    class Marksheet extends Student_1{
    int maths, physics, chemistry;
    Marksheet(String n, int m, int ph, int ch){
    super(n);
    maths = m;
    physics = ph;
    chemistry = ch;
    }
    void display(){
    System.out.println("Name: " + Name);
    int total = maths + physics + chemistry;
    System.out.println("Total Marks: " +total);
    }
    public static void main(String[] args){
    Marksheet ms = new Marksheet("Rahul",90,92,88);
    ms.display();
    }
    }