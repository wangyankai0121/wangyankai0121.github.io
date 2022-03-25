## Не робейте

不要害怕。最重要的事：要过正常的生活，不要做激情的奴隶。不然，有什么好处呢？不论浪头把您卷到哪儿，还不是一样的糟。一个人即使站在一块石头上，他也站得稳的。

Не робейте. Главное дело: жить нормально и не поддаваться увлечениям. А то что пользы? Куда бы волна ни понесла — всё худо; человек хоть на камне стой, да на своих ногах.

И. С. 屠格涅夫《初恋》

```c
bool hasCycle(struct ListNode *head) {
    if(head==NULL||head->next==NULL){
        return false;
    }
    struct ListNode *slow=head;
    struct ListNode *fast=head->next;
    while(fast!=slow){
        if(fast==NULL||fast->next==NULL){
            return false;
        }
        slow=slow->next;
        fast=fast->next->next;
    }
    return true;
}
```
