# Array-of-size-N-print-second-largest-element-from-an-array.
N = 6
Arr[] = {12, 35, 1, 10, 34, 1}
Output: 34
Explanation: The largest element of the 
array is 35 and the second largest element
is 34.



class Solution{
public:	
	// Function returns the second
	// largest elements
	int print2largest(int arr[], int n) {
	    
	    int max=arr[0]; int  min=-1;
	    
	    for(int i=0; i<n; i++)
	  
	    if(arr[i]>max){
	        max=arr[i]; //update
	    }
	        
	         for(int i = 0; i < n; i++) {
           if(arr[i] < max && arr[i] > min)
               min = arr[i]; //update
       }
       
       
       return min;
	    
	}
};
