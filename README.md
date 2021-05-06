(1)-ans:- 
function question(array){
let arr=[];
for(let i=0;i<array.length;i++){
if(i%2===0){
arr.push(array[i]);
}
return arr;
}
}

2-ans (a):-
public static int maxOnes(int[] arr){
		int count = 0;
		int max = 0;
		for(int i = 0; i < arr.length; i++){
			if(arr[i] == 0)
				count = 0;
			else
				count++;
			max = count > max ? count : max;
		}
		return max;
	}
  
(b):-

public static int maxNumberOf1s(String str) {
		if (null == str || str.isEmpty() || !str.contains("1")) {
			return 0;
		}
		int count = 0;
		int curCount = 0;
		for (int i = 0; i < str.length(); i++) {
			if (str.charAt(i) == '1') {
				if (curCount == 0) {
					curCount = 1;
				} else {
					curCount++;
				}
				count = Math.max(curCount, count);
			} else {
				curCount = 0;
			}
		}

		return count;
	}
(3) ans:-


// C++ program to Find the two repeating
// elements in a given array
#include<bits/stdc++.h>
using namespace std;
 
void printRepeating(int arr[], int size)
{
    int i, j;
    printf(" Repeating elements are ");
    for(i = 0; i < size; i++)
        for(j = i + 1; j < size; j++)
        if(arr[i] == arr[j])
            cout << arr[i] << " ";
}
 
// Driver Code
int main()
{
    int arr[] = {4, 2, 4, 5, 2, 3, 1};
    int arr_size = sizeof(arr)/sizeof(arr[0]);
    printRepeating(arr, arr_size);
}


(4) ans:-

public class Person {
	private String name;
	private String about;
	private int birthYear;
	
	public Person(String name, String about, int birthYear) {
		this.name = name;
		this.about = about;
		this.birthYear = birthYear;
	}

	public String getName() {
		return name;
	}

	public String getAbout() {
		return about;
	}

	public int getBirthYear() {
		return birthYear;
	}
}

(5) ans:-

var list = {
  "abc": 4, 
  "ab2": 10, 
  "abc3": 5, 
  "abc5": 6
};



list = {
  "abc": 4, 
  "ab2": 10, 
  "abc3": 5, 
  "abc5": 6
};
