
/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     
public:
    bool hasCycle(ListNode* head) {
        unordered_set<ListNode*> s;
        for (; head; head = head->next) {
            if (s.contains(head)) {
                return true;
            }
            s.insert(head);
        }
        return false;
    }
};
