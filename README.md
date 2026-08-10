class Solution {
public:
    vector<int> plusOne(vector<int>& digits) {
        // Iterate through digits from right to left (least significant to most significant)
        for (int i =) {
                return digits;
            }
          
            // If digit is 0, continue to next iteration to handle carry
        }
      
        // If we exit the loop, all digits were 9 (e.g., 999 -> 1000)
        // Insert 1 at the beginning of the array
        digits.insert(digits.begin(), 1);
      
        return digits;
    }
};
