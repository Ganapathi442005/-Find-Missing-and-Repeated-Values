https://leetcode.com/problems/find-missing-and-repeated-values/description/?envType=problem-list-v2&envId=matrix&difficulty=EASY



class Solution {
public:
    vector<int> findMissingAndRepeatedValues(vector<vector<int>>& grid) {
       unordered_map<int,int> mp;
        int n= grid.size();
        for(int i=0;i<grid.size();i++)
        {
            for(int j=0;j<grid.size();j++)
            {
                mp[grid[i][j]]++;
            }
        }
        vector<int> a;
        for(int i=1;i<=(n*n);i++)
        {
            if(mp[i]>1)
            {
                a.push_back(i);
            }
        }
        for(int i=1;i<=(n*n);i++)
        {
            if(mp[i]==0)
            {
                a.push_back(i);
            }
        }
        return a; 
    }
};
