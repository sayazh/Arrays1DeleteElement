# Arrays1DeleteElement
Arrays1DeleteElement
import java.util.Arrays;
import java.util.Scanner;

public class Arrays1DeleteElement {

	public static void main(String[] args) {
       
        int[] intArr = {1, 8, 5, 8, 7, 3, 8};
        System.out.print(Arrays.toString(deleteR(intArr,8)));
        
        
	}    
      public static int[] deleteR(int[] arr, int element) {
    	  int count=0;
    	  
    	 
    	  for(int i = 0; i<arr.length;i++) {
    		  if(arr[i]== element) {
    			  count++;
    		  }
    	  } if(count==0) {
    		  return arr;
    	  } 
    	   
    	  int index=0;
    	  int[] newArr = new int[arr.length-count];
    	  for(int r : arr) {
    		  if(r!=element) {
    			  newArr[index]=r;
    			  index++;
    		  }
    	  }
    	   return newArr;
      }
}
    	     
    	     
    	     
