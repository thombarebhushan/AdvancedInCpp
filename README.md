# Some Unknown cpp Algorithm's

1.Partial Sort and nth Element<br> 
2.Ordered Set<br>

# 1.Partial Sort and nth Element

/*
In C++, a partial sort is an algorithm that partially sorts a range of elements in a container, such as a vector or an array. 
Unlike a complete sort, which orders all elements, a partial sort rearranges only a portion of the elements so that the smallest 
(or largest) elements are sorted up to a certain point. 
std::partial_sort has a time complexity of 𝑂(𝑁 log𝐾) where N is the number of elements and K is the number of elements to sort
*/
```cpp
partial_sort(vec.begin(), vec.begin() + 5, vec.end());
/*
Partitioning: Elements before 5th are less than or equal to the element at nth,
and elements after nth are greater than or equal to it
*/

vec = {10, 2, 8, 6, 7, 5, 1, 3, 4, 9};

nth_element(vec.begin(), vec.begin() + 4, vec.end()); 
/*
Avg .TC => O(n)

Worst .TC => O(n^2)
take the nth element at its correct position aftter sort
*/
```


# 2.Ordered Set
```cpp
#include<ext/pb_ds/assoc_container.hpp>
#include<ext/pb_ds/tree_policy.hpp>
using namespace __gnu_pbds;
//                         less<int> 
//                         greater<int>                 
typedef tree<int,null_type,less_equal<int>,rb_tree_tag,tree_order_statistics_node_update>s1;
int main(){
  s1 s; 
}

*s1.order_of_key(6)
/*The order_of_key function is used to find the number of
elements that are strictly less than a given element in a sorted container.
*/

s1.find_by_order(2)
/*
The find_by_order function is used to find the element at a given index in a sorted container.
It allows access to the element at a specific position in the sorted sequence.
*/
```
