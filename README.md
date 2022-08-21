# Understanding Array methods.

## Mutable array methods:  Array methods that makes changes in original array. 

* ### push 
   This method pushes a new item to the end of an array.
   
     #### Examples:
     * console.log([1,2].push(3)) ==> [1,2,3]
     
* ### reverse 
   This method will reverse the array elements.
   
     #### Examples:
     * console.log([1,2].reverse()) ==> [2,1]

* ### shift 
   This method removes the first item in an array.
   
     #### Examples:
     * console.log([1,2,3].shift()) ==> [2,3]

* ### splice
   This method lets us to change the content of array by removing or replacing existing elements with new ones.
   
  * arr.splice(startIndex)  **delete all items from startIndex**
  * arr.splice(startIndex, deleteCount)  **delete deleteCount items from startIndex**
  * arr.splice(startIndex, deleteCount, addItem1)  **delete deleteCount items from startIndex and addItem1 to its position**
  * arr.splice(startIndex, deleteCount, item1, item2, tillItemN)   **delete deleteCount items from startIndex and addItem1 to tillItemN to its position**

* ### unshift
  This method adds n number of elements at the beginning of the array.
  
  #### Examples:
  * console.log([3].unshift(1,2)) ==> [1,2,3]
  
* ### pop
  This method removes and returns the last element of an array.
  
  #### Examples:
  * console.log([1,2,3,3].pop()) ==> [1,2,3] 
  
  
## Immutable array methods:  Array methods that dose not makes changes in original array. 

* ### join 
  Joins the elements of array based on the string passed as parameter passed and convert it into String.

  #### Examples:
  * console.log([x,y,z].join(''))  ==> "xyz" 
  * console.log([1,2,3].join(',')) ==> "1,2,3"
  * console.log([abc,xyz].join('-') ==> "abc-xyz"

* ### flat 
  This method returns the array having sub-array elements merged to the specified depth.

  #### Examples:
  * console.log([[1, 2], [3, 4], 5].flat())  ==> [1,2,3,4,5] 


* ### indexOf
  This method returns the first matching index of specified item in the array.

  #### Examples:
  * console.log([1,2,3].indexOf(3)) ==> 2 

* ### lastIndexOf
  This method returns the last matching index of specified item in the array.
  
  #### Examples:
  * console.log([1,2,3,3].indexOf(3)) ==> 3 
  
* ### includes
  This method checks if array contains the specified element and returns boolean vaule.
  
  #### Examples:
  * console.log([1,2,3,3].includes(3)) ==> true 


* ### every
  This method iterates oevr each element in the array checks if the specified condition is satsfied or not and returns boolean vaule.
  
  #### Examples:
  * console.log([1,2,3,3].every(e => e > 0)) ==> true
  * console.log([1,2,3,3].every(e => e < 0)) ==> false 

* ### find
  This method returns the first element that statsfies the specified condition.
  
  #### Examples:
  * console.log([1,2,3,3].find(e => e > 1)) ==> 2


* ### findIndex
  This method returns the index of the first element in the array that satsfies the condition. Otherwise, -1.

  #### Examples:
  * console.log([1,2,3,3].find(e => e > 1)) ==> 1 // index of 2

* ### filter
  This method creats a new array containing the elements that satsfies the test condition.
  
  #### Examples:
  * console.log([1,2,3,3].filter(e => e > 1)) ==> [2,3,3] 

* ### forEach
  It iterates once for each element of an array.

  #### Examples:
  * let result = []
    [1,2,3,3].forEach(e => result.push(e+1))
    console.log(result) ==> [2,3,4,4]

* ### map
  This method calls the specified function for every element and returns a new array.
  
  #### Examples:
  * console.log([1,2,3,3].map(e => e - 1)) ==> [0,1,2,2] 


* ### reduce
  This method executes a provided function for each value and reduces the array to a single value.

  #### Examples:
  * console.log([1,2,3,3].reduce((acc,curr) => acc + curr)) ==> 9


* ### slice
  This method creats a new array containing the elements of part of the given array.

  #### Examples:
  * console.log([1,2,3,3].slice(0,2) ==> [1,2,3] 

* ### some
  This method determines if any one element in the array satsfies the condition and return boolean value.

  #### Examples:
  * console.log([1,2,3,3].some(e => e > 4) ==> false
  * console.log([1,2,3,3].some(e => e > 2) ==> true 

