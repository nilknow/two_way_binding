# two ways binding
try to implement vue2's and vue3's two-way binding on my own 
in order to have a deep understand of two-way binding 


## step by step
1. view changes => data changes
    add a eventListener to view object (like an input element).
2. data changes => view changes
    set setter of data, let the setter function modify the corresponded element
3. found that I can't show the properties in chrome console
   Object.defineProperty modify the prototype of this class, but not the instance
   When you just use console.log() to get debug output you only 
   see the instance's own properties, not the ones on the prototype.
   [Why does my property disapear after Object.defineProperty in decorator?](https://stackoverflow.com/questions/46979524/why-does-my-property-disapear-after-object-defineproperty-in-decorator)
