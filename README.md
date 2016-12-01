# ACD_JAVAB2_Session_6_Assignment_4
package Session6_Assignment;
import java.util.Arrays;
import java.util.Scanner;

public class Array {
	public static void main(String[] args) {

		   // initializing unsorted int array
		
	       int arr[],n,x;
	       Scanner sc = new Scanner(System.in);
	       System.out.println("The length of single dimentional array");
	       n = sc.nextInt();
	       arr = new int[n];
	       for(int i=0;i< arr.length;i++){
	    	   System.out.println("enter the values of array");
	    	   x = sc.nextInt();
	    	   arr[i] = x;
	       }
	       for(int i=0;i< arr.length;i++){
	    	   System.out.println("array values"+ " " + arr[i]);
	    	  
	       }
	       System.out.println("enter searchvalues:");
	      int m =sc.nextInt();
	      Arrays.sort(arr);
	      for(int num : arr){
	    	   System.out.println("display array after sort" + num);
	    	      			   
	      }
	     int  numfound = Arrays.binarySearch(arr,m);
	      if (numfound < 0){
	    	  System.out.println("the number:" +" "+ m + "  not found in array");    	    
	      }
	      else{
	     System.out.println("The number is found in array and  index of element of" + m +"is: "+ numfound);
	}
	}
}
