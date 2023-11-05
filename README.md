# Kids-With-the-Greatest-Numbers-of-Candies-using-Java-Leetcode

    class Solution {
        public List<Boolean> kidsWithCandies(int[] candies, int extraCandies) {
            List<Boolean> list = new ArrayList<Boolean>();
            for(int i = 0;i<candies.length;i++){
                int temp =candies[i]+extraCandies;
                list.add(i,true);
                for(int j =0;j<candies.length;j++){ 
                    
                    if(candies[j]>temp){
                        list.set(i,false);
                        break;
                    }
                }
                
    
            }
            return list;
        } 
    }
