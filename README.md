Whenever we declare a vector like:

          1- vector<int> v; 
Here, we do not specify the size of our vector.
 Whenever we just want to add an element we just 
push it into the vector using the  v.push _ back
(val)  function (where val is the value you want 
to push).

Suppose you haven't added any elements into the 
vector. Now, if you go on access any element 
position like  v[0]  or  v[7]  like one can when
 he declares an array, you will get a runtime 
error. Why? Because vectors are dynamic in nature.
 Since, you haven't declared any size or pushed 
any element it's size is zero. So no element 
exists right now.

But if you declare it using:

       2- vector<int> v(N); 
The compiler would there only create an dynamic
 array of size N with all values initialized to 
zero. Now, you can randomly access elements but 
only from  v[0]  to  v[N−1] . But, if you want 
to add more than N elements then you can anytime 
use the push _ back()  function to add elements.

Now, coming to

       3-vector<int> v[N]; 
It creates a static array of N vectors of the 
first type i.e.  v[0]  is now a whole new and 
different vector than v[1] which is totally 
different than  v[2]  and so on. If you want 
to push a value into the 1st vector that is 
 v[0] , you will do it by  v[0].push _ back(val) 
. To access that element you will call it by 
 v[0][0] (kind of a 2d matrix, isn't it?!).
 So, basically it is an array of initially empty 
vectors to which you can add elements. These are
 very useful while you want to implement graphs
 where each node has it's own vector and the
 nodes to which it is joined are pushed into
 that particular node's vector.

I hope you get the point!
