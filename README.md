# problem 1 Score of a String
class Solution {
    public int scoreOfString(String s) {
        int sum=0;
        for(int i=0;i<s.length()-1;i++){
            char ch1=s.charAt(i);
             char ch2=s.charAt(i+1);
             sum+=Math.abs((ch1+0)-(ch2+0));
        }
        return sum;
    }
}
# problem 2 Concatenation of Array
class Solution {
    public int[] getConcatenation(int[] nums) {
        int[]arr=new int[nums.length*2];
        for(int i=0;i<nums.length;i++){
            arr[i]=nums[i];
             arr[i+nums.length]=nums[i]; 
        }
        return arr;
    }
}
# problem 3 Contains Duplicate
class Solution {
    public boolean hasDuplicate(int[] nums) {
        HashSet<Integer> set=new HashSet<>();
        for(int n:nums){
           if( set.contains(n))
            return true;
                   set.add(n);
        }
         return false;
            }
}
