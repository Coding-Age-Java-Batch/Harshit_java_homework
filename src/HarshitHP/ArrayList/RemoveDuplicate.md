import java.util.*;
public class RemoveDuplicate {
static void main(String[] args) {
ArrayList<Integer> list = new ArrayList<>();

         list.add(1);
         list.add(2);
         list.add(2);
         list.add(3);
         list.add(3);

         ArrayList<Integer> uniqueList = new ArrayList<>();

         for(int i = list.size()-1; i>=0; i--){
             if(uniqueList.contains(list.get(i))){
                 list.remove(i);
             }
             else{
                 uniqueList.add(list.get(i));
             }
         }
       ArrayList<Integer> finalList = new ArrayList<>();
         for(int i = uniqueList.size()-1; i>=0; i--){
             finalList.add(uniqueList.get(i));
         }
        System.out.println("Final List: "+finalList);
    }
}
