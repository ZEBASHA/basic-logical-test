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
