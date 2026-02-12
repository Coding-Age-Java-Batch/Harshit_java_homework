public class Book {
String title;
String author;
double price;

    public Book(String tl,String ar,double pc){
        title = tl;
        author = ar;
        price = pc;
    }
    Book(String tl,String ar){
        title = tl;
        author = ar;
        price = 250;
    }

    void details(){
        System.out.println("Title: " +title);
        System.out.println("Author: " +author);
        System.out.println("Price: " +price);
    }

    static void main(String[] args) {
        Book b1 = new Book("java Programming","Jhon Doe");
        b1.details();
    }
}
