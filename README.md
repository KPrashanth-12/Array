# Array
//Code for largest and smallest numbers in array



import java.util.Scanner;
public class Array {
    public static int linearSearch(int numbers[], int key){
        for(int i=0; i<numbers.length; i++){
            if(numbers[i] == key){
                return i;
            }
        }
        return -1;
    }
    public static int getLargest(int numbers[]){
        int largest = Integer.MIN_VALUE;
        int smallest = Integer.MAX_VALUE;
        for(int i = 0; i <numbers.length; i++){

        
      if(largest < numbers[i]){
            largest = numbers[i];
        }
        if(smallest > numbers[i]){
            smallest = numbers[i];
        }
    }
    System.out.println("Smallest number is :" + smallest);
      return largest;
}

    public static void main(String[] args){
        int numbers[] = { 4,3,7,8,2,1,6 };
        System.out.println("the largest number is : " + getLargest(numbers));
        
    
    }
    
}
