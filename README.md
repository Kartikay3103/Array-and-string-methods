# Array and String Methods

# Array

* An array is a special variable, which can hold more than one value
* Array is an object that represents a collection of similar type of elements


# Array Methods

### for each()
  * This method can help you to loop over array's item.
  * Method calls a function for each element in an array.
  * The forEach() method is not executed for empty elements.
  

        const arr =[1,2,3,4,5,6];

        arr.forEach(item => {
         console.log(item);

        }); 
  

### Includes()
* This method check if array includes the item passed in the method.
*  The includes() method determines whether an array includes a certain value among its entries, returning true or false as appropriate.
    
     `Note: When comparing strings and characters, includes() is case-sensitive. `



        const array1 = [1, 2, 3];

       console.log(array1.includes(2));
        // expected output: true

       const pets = ['cat', 'dog', 'bat'];

       console.log(pets.includes('cat'));

       // expected output: true
        console.log(pets.includes('at'));
       // expected output: false


### filter()

* The filter() method creates a new array with all elements that pass the test implemented by the provided function.
* The filter() method does not execute the function for empty elements.

* The filter() method does not change the original array.

            
       const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

      const result = words.filter(word => word.length > 6);

       console.log(result);



### Map()

* The map() method creates a new array populated with the results of calling a provided function on every element in the calling array. 
* map() creates a new array from calling a function for every array element.
* map() calls a function once for each element in an array.
* map() does not change the original array.

            const array1 = [1, 4, 9, 16];
            // pass a function to map
            const map1 = array1.map(x => x * 2);
            console.log(map1);


### reduce()
* The reduce() method executes a user-supplied "reducer" callback function on each element of the array, in order, passing in the return value from the calculation on the preceding element. The final result of running the reducer across all elements of the array is a single value. 
* The reduce() method executes a reducer function for array element.
* The reduce() method returns a single value: the function's accumulated result.
* The reduce() method does not execute the function for empty array elements.

           
       const array1 = [1, 2, 3, 4];

      // 0 + 1 + 2 + 3 + 4
        const initialValue = 0;
        const sumWithInitial = array1.reduce(
        (previousValue, currentValue) => previousValue + currentValue,
         initialValue
            );

         console.log(sumWithInitial);

### Some()

* The some() method checks if any array elements pass a test (provided as a function)
* The some() method executes the function once for each array element:
  
     1. If the function returns true, some() returns true and stops.
     2. If the function returns false, some() returns false and stops.
   
* The some() method does not execute the function for empty array elements.

* The some() method does not change the original array.


       const array = [1, 2, 3, 4, 5];

      // checks whether an element is even
        const even = (element) => element % 2 === 0;

        console.log(array.some(even));

### sort()
* The sort() sorts the elements of an array.
* The sort() overwrites the original array.
* The sort() sorts the elements as strings in alphabetical and ascending order.


       const months = ['March', 'Jan', 'Feb', 'Dec'];
        months.sort();
        console.log(months);
         // expected output: Array ["Dec", "Feb", "Jan", "March"]

          const array1 = [1, 30, 4, 21, 100000];
           array1.sort();
          console.log(array1);
          // expected output: Array [1, 100000, 21, 30, 4]



# String

* The String object is used to represent and manipulate a sequence of characters. 

# String Method

### length

* The length property returns the length of a string.
* The length property of an empty string is 0.

         <!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.length;
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>

### to LowerCase
* The toLowerCase() method converts a string to lowercase letters.
* The toLowerCase() method does not change the original string.

<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.toLowerCase();
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>



### to UpperCase
* The toUpperCase() method converts a string to uppercase letters.
* The toUpperCase() method does not change the original string.

<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.toUpperCase();
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>

### includes()
* The includes() method returns true if a string contains a specified string.
* Otherwise it returns false.
* The includes() method is case sensitive.

<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.include("great);
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>

### startsWith()
* The startsWith() method returns true if a string starts with a specified string.
* Otherwise it returns false.
* 
<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.startsWith("ipt");
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>

### endsWith()

* In JavaScript, endsWith() is a string method that is used to determine whether a string ends with a specific sequence of characters. Because the endsWith() method is a method of the String object, it must be invoked through a particular instance of the String class.


<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.endsWith("age");
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>

### Search()
* The search() method matches a string against a regular expression 
* The search() method returns the index (position) of the first match.
* The search() method returns -1 if no match is found.
* The search() method is case sensitive.

<!DocTYPE html>
         <html>
         <head>
        <title>JavaScript</title>
        <script>
        var str = "JavaScript is a great Language";
        var a = str.search("is");
       document.write(a);
       </script>
      </head>
       <body>
       </body>
         </html>



# Reference

https://www.w3schools.com/jsref/jsref_search.asp

https://www.javatpoint.com/
