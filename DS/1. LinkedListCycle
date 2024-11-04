class Solution {
public:
    bool hasCycle(ListNode *head) {
        if(!head || head -> next == nullptr || head -> next -> next == nullptr)
            return false; // if the list is empty 

        ListNode* slow = head;
        ListNode* fast = head -> next;

        while(fast != nullptr)
        {
            if(slow == fast)
                return true;   // if slow meets fast 

            if(fast -> next == nullptr || fast -> next -> next == nullptr)
                return false;  // to avoid any errors 
            
            slow = slow -> next; 
            fast = fast -> next -> next; 
            
        }

        return false;
    }
};