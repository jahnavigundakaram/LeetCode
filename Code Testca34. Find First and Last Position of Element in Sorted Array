class Solution {
public:
    vector<int> searchRange(vector<int>& nums, int target) {
        vector<int> ans(2,-1);
        
        if(nums.size()==0)
            return ans;
        
        int left = 0 , right = nums.size()-1;
        
        auto it = find(nums.begin(),nums.end(),target);
        if(it == nums.end())
            return ans;
        
        
        while(left <= right ){
            if(nums[left] == target) //find starting pos
                ans[0] = left;
            if(nums[right] == target)//find ending pos
                ans[1] = right;
            
            if(ans[0]!=-1 && ans[1]!=-1)
                break;
 
            if(ans[0] == -1)
                left ++;
            if(ans[1] == -1)
                right --;
        }
        
        return ans;
    }
};
