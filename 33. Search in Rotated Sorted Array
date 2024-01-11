class Solution {
public:
    
    
    int search(vector<int>& nums, int target) {
        int left =0, right= nums.size()-1;
        int mid = left + (right - left)/2 ;
        if(nums.size()==1)
            if(nums[0]!=target)
                return -1;
        while(left < right){
            
            mid = left + (right - left) /2 ;
            cout << left << " mid:" << mid << " " <<right << endl;
            if(nums[mid] == target)
                return mid;
            if(nums[mid] < nums[right]){ // mid ~ right是排序好的
                if(target > nums[mid] && target <= nums[right]){
                    left = mid+1;
                    //cout << left;
                }else{
                    right = mid-1;
                }
            }else{//left ~ mid 是排序好的
                if(target < nums[mid] && target >= nums[left]){
                    right = mid-1;
                    
                }else{
                    left = mid + 1;
                }
            }
            if(mid==right || mid == left){
                if(nums[mid] != target)
                    return -1;
            }
            if(left == right && nums[left]!= target)
                return -1;
                
        }
        
        return left;
    }
};
