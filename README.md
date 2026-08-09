
class Solution {
            dfs(node->right);                // Traverse right subtree
        };
      
        // Start the traversal from root
        dfs(root);
      
        return result;
    }
};
