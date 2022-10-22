/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    ListNode* addTwoNumbers(ListNode* l1, ListNode* l2) {
        ListNode* resultant = new ListNode(0);
        ListNode* curr = resultant;
        int sum = 0;
        int total = 0;
        int x;
        int y;
        while(l1 != nullptr || l2 != nullptr || total != 0) {
            x = (l1 != nullptr) ?l1->val: 0;
            y = (l2 != nullptr) ?l2->val: 0;
            sum = total + x + y;
            total = sum / 10;
            curr->next = new ListNode (sum % 10);
            curr = curr->next;
            l1 = (l1 != nullptr)? l1->next: nullptr;
            l2 = (l2 != nullptr)? l2->next: nullptr;
        }
        return resultant->next;
    }
};
