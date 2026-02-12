    class VolumeCalculator {
    int volume(int side){
    return side * side * side;
    }

     int volume(int length, int breadth, int height){
         return length * breadth * height;
     }

     int volume(double radius, double heigth){
         return (int) (3.14 * radius * radius * heigth);
     }
     public static void main(String[] args){
         VolumeCalculator vc = new VolumeCalculator();

         System.out.println("Volume of cube: " +vc.volume(3));
         System.out.println("Volume of cuboid: " +vc.volume(4,5,6));
         System.out.println("Volume of cylinder: " +vc.volume(5.0,4.0));
     }
    }
