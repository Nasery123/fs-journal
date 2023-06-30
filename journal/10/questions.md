# CSharp and SQL Fundamentals

1.  What is the purpose of a `namespace`?

> |to provide accessiblity for other other files. does something like import and export |

2.  What is the difference between a `class` and an `interface`?

> | a class is a template to create an object and interface defines a set of members that a class must implement |

3.  What is the method that returns an instance of a class, yet it has no return type?

> | it is a constructor that does not have a return anything but it is a method. |

5.  In the Car example what is the access modifier of the `Start()` method?

```c#
abstract class Car
{
  public string Start()
  {

    return "Vroooom";

  }
}
```

> | the modifier for the start is public |

6.  In the Car example what is `string` an indication of?

> | it shows that return data type of start |

7.  In the Car example what is `abstract` preventing?

> | the abstract is used to prevent from creating instance of a class directly using new. |

8.  In a SQL table, what is the difference between information in a row and information in a column?

> | the information in column shows the table information and a specifc information of that table for every single row. but the the row show the complete information related to each other. |

9.  Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

> | CREATE TABLE charecter (

    id int NOT NULL PRIMARY KEY AUTH_INCREMENT,
    name VARCHAR(255) NOT NULL,
    age INT NOT NULL,
    description VARCHAR(255) NOT NULL,

) |

10. In SQL how can you query more than a single table? Provide an example.

> | SELECT Customers.CustomerName
> FROM Customers
> INNER JOIN Orders
> ON Customers.CustomerID = Orders.CustomerID |
