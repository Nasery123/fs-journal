# A bit more CSharp and SQL

1. What does **_inheritance_** accomplish for us in C#?

> | inheritance enables us to access some properties that is not directly in the class. but through a relationship that creates it enables us to use properties of its parent's class |

2. How does **_member inheritance_** work in C#? Does a `Class` inherit all members of the base `Class`?

> | the class inherites all members of the base class and modifies it to use the way it needs. only constructor from the inherited class excludes when making the inheritance relationship |

3. How does **_accessibility_** affect inheritance?

> | there are three situation that defines the accessibility, public, protected, internal and private. there is no problem accessing public and private methodes when inheriting. However if the method is internal files should be at the same assembly inorder to be accessable. and private methodes are only usable inside class itself and can not be inherited. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

> | the primary key is a column of unique thing that is related to the data in the sql. on the other hand the foreign key is a unique thing that makes relationship between two tables and refers to the primary key of the other table. |

5. What is an **_alias_**?

> | an alternative name to the sql table. |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

```SQL
CREATE TABLE doctors (
  id INT NOT NULL AUTO_INCREMENT,
  -- CODE OMITTED
  PRIMARY KEY (id)
)

CREATE TABLE patients (
  id INT NOT NULL AUTO_INCREMENT,
  -- CODE OMITTED
  PRIMARY KEY (id)
)

CREATE TABLE patient_doctors (
  id INT NOT NULL AUTO_INCREMENT,
  doctorId INT NOT NULL,
  patientId INT NOT NULL,

  FOREIGN KEY (doctorId)
    REFERENCES doctors(id),
  FOREIGN KEY (patientId)
    REFERENCES patients(id),
)

```

> | SELECT

patients.\* pat,
FROM patient
JOINT patient_doctors pdr on pdr.id = pd.patientId
JOINT doctors doc ON pdr.doctorId = doc.id
WHERE doc.id = @id |
