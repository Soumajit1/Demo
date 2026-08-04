class Solution {
public:
    int maxRotateFunction(vector<int>& nums) {
        int n = 
        }

        long long ans = f;

        for (int i = n - 1; i > 0; i--) {
            f = f + sum - 1LL * n * nums[i];
            ans = max(ans, f);
        }

        return (int)ans;
    }
};
