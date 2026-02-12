class Product {
int productId;
String productName;
double price;

     Product(int id, String Pn, double pc){
         productId = id;
         productName = Pn;
         price = pc;
     }
     void applyDiscount(double discountPercent){
         double discountAmount = price * discountPercent / 100;
         price = price - discountAmount;

         System.out.println("Updated price after: " + discountPercent + "% discount : " + price);
     }

     public static void main(String[] args){
         Product p1 = new Product(101,"Laptop",50000);
         p1.applyDiscount(10);
     }
}
