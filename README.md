class Solution {
private:
    vector<int> Next(string str) {
        vector<int> n(str.length());
        n[0] = -1;
        int i = 0, pre = -1;
        int len = str.
p() && k < haystack.length()) {
                if (haystack[k] != needle[j]) {
                    if (n[j] >= 0) {
                        j = n[j];
                        continue;
                    } else
                        break;
                }
                ++k, ++j;
            }
            if (j >= needle.length())
                return k - j;
        }

        return -1;
    }
};
