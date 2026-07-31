/**
 * Definition fo\
    bool isValidBST(TreeNode* root) {
        TreeNode* prev = nullptr;
        function<bool(TreeNode*)> dfs = [&](TreeNode* root) {
\
            return dfs(root->right);
        };
        return dfs(root);
    }
};
