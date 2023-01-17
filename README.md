# assignment
1.Write a program to find largest and smallest number in array using loops from 
arr=[ 43, 56, 23, 89, 88, 90, 99, 652]


#CODE
public class solution{
 public static void main(String[] args) {
  int num[] = new int[]{43, 56, 23, 89, 88, 90, 99, 652};
  int small = num[0];
  int large = num[0];
  for (int i = 1; i < num.length; i++) {
   if (num[i] > large)
    large = num[i];
   else if (num[i] < small)
    small = num[i];
  }
  System.out.println("Largest Number is : " + large);
  System.out.println("Smallest Number is : " + small);
 }
}

OUTPUT:
Largest Number is : 652
Smallest Number is : 23





2.Write a program to create two arrays which contains even number in one array and odd numbers in another array from given array.
array = [1,2,3,4,5,6,7,8,9,10]


#CODE
import java.util.*;
class main {
    public static void main(String[] args) {
    Scanner sc=new Scanner(System.in);
            int n=sc.nextInt();
            int arr[]=new int[n]; 
            ArrayList<Integer>odd = new ArrayList<>();
            ArrayList<Integer>even = new ArrayList<>();
            for(int i=0;i<n;i++)
        {
            arr[i]=sc.nextInt();
        }
        for(int i=0;i<n;i++)   
        {
            if(arr[i]%2==0){
            even.add(arr[i]); 
             }
        else{
            odd.add(arr[i]);
        }
        }
         for(int i=0;i<even.size();i++){
            System.out.print(even.get(i)+" "); 
        }
         System.out.println(" ");
        for(int i=0;i<odd.size();i++){
            System.out.print(odd.get(i)+" ");}
    }
}

OUTPUT:
Value:10
ArrayList:1 2 3 4 5 6 7 8 9 10
Even:2 4 6 8 10
Odd:1 3 5 7 9





3.write a program to create an array with all unique numbers from a given array of arrays
arr=[[1, 2, 3], [3,4,5], [8,9,10]]


#CODE
import java.util.*;
class main{
	public static void main(String[] args){
		int[][] arr = { { 1, 2, 3 },
                        { 3,4,5 },
                        { 8,9,10 } };
        LinkedHashSet<Integer> set
            = new LinkedHashSet<Integer>();
        for(int i=0;i<3;i++){
        	for(int j=0;j<3;j++){
        		set.add(arr[i][j]);
        	}
        }
        System.out.println(set);
        
    }
}

OUTPUT:
[1, 2, 3, 4, 5, 8, 9, 10]





4. Write a program to find all the author names from the array from given below
arrayData=
[  
   { author: 'Bill Gates', title: 'The Road Ahead', libraryID: 1254}, 
   { author: 'Steve Jobs', title: 'Walter Isaacson', libraryID: 4264}, 
   { author: 'Suzanne Collins', title: 'Mockingjay: The Final Book of The Hunger Games', libraryID: 3245}
];


#CODE(JAVASCRIPT)

var arrayData=
[  
   { author: 'Bill Gates', title: 'The Road Ahead', libraryID: 1254}, 
   { author: 'Steve Jobs', title: 'Walter Isaacson', libraryID: 4264}, 
   { author: 'Suzanne Collins', title: 'Mockingjay: The Final Book of The Hunger Games', libraryID: 3245}
]; 

for (var i = 0; i < arrayData.length; i++) 
   {
    console.log(arrayData[i].author);
   }
   
OUTPUT:
Bill Gates
Steve Jobs
Suzanne Collins
