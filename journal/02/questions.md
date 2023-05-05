# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | let is a key word that is used for variables we might change its value. and const is a key word that is used for non-changing value variables |

02. What is the definition of a function?

    > | function is a block of codes that can be used over and over again. this block of code has specific rules that should be defined using (function) keyword and invoking the function |

03. What are the `SOLID` principles?

    > | ANSWER HERE |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit.splice(1,1)|

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > | you.friends = [them]
    them.friends = [you] |

06. Give an example of a JavaScript `Conditional`:

    > | if(num % 2 ===0 ){
        return true
    }
    return false;
     |

07. What is the main difference between `parameters` and `arguments`?

    > | parameters are used to define a function. they are created when the function is defined. However, arguments are the values a function recieves instead of parameters |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | using debugger enables us to analyze our code step by step. |

09. What is the difference between a `primitive` value and a `reference` value?

    > | Primitive values are string, number, bolean, undefined, null but reference vlues are the type of value which we access them indirectly, for instance and element of arry of an element of an object.|

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for (let i = -100; i <= 100; i++){
        console.log(i)|
