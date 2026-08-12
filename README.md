/**
 * Definition for a binary tree node.
 * struct TreeNode {
 *     int val;
 *     TreeNode
class Solution {
public:
    int maxPathSum(TreeNode* root) {
        int ans = -1001;
        function<int(TreeNode*)> dfs = [&](TreeNode* root) {
            if (!root) {
                return 0;
            } + right + root->val);
            return root->val + max(left, right);
        };
        dfs(root);
        return ans;
    }
};
