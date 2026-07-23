/**
 * Definition for singly-linked list.
  struct ListNode {
     int val;
      stNode *next;
   ListNode() : va
    ListNode* rotateRight(ListNode* head, int k) {
        if (!head || !head->next) 
        }
        ListNode* fast = head;
        ListNode* slow = head;
        while (k--) {
            fast = fast->next;
        }
        while (fast->next) {
      fast = fast->next;
            slow = slow->next;
        }
        ListNode* ans = slow->next;
        slow->next = nullptr;
        fast->next = head;
        return ans;
    }
};
