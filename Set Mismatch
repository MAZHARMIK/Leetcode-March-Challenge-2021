class Solution {
public:
    vector<int> findErrorNums(vector<int>& nums) {
        int n = nums.size();
        int miss = 0, dup = 0;
        
        map<int, int> mp;
        for(int x:nums) {
            mp[x]++;
        }
        
        for(int i = 1; i<=n; i++) {
            if(mp.count(i)) {
                if(mp[i] == 2)
                    dup = i;
            } else
                miss = i;
        }
        
        return {dup, miss};
    }
};
