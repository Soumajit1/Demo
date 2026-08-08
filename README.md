
class Solution {
public:
    /**
     * Performs inorder traversal of a binary tree
     * @param root - The root node of the binary tree
     * @return A vector containing the values of nodes in inorder sequence
     */
    vector<int> inorderTraversal(TreeNode* root) {
        // Vector to store the result of inorder traversal
        vector<int> result;
      
        // Lambda function for recursive depth-first search
        // Captures result vector by reference to modify it
        function<void(TreeNode*)> dfs = [&](TreeNode* node) {
            // Base case: if node is null, return
            if (!node) {
                return;
            }
          
            // Inorder traversal: Left -> Root -> Right
            dfs(node->left);                // Traverse left subtree
            result.push_back(node->val);    // Process current node
            dfs(node->right);                // Traverse right subtree
        };
      
        // Start the traversal from root
        dfs(root);
      
        return result;
    }
};
