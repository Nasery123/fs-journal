# Intro to Server side concerns with JavaScript
01. What do the letters of the acronym `CRUD` stand for?

  > | create, read, update and delet |

02. Each action that `CRUD` represents maps to an HTTP request. What HTTP request does each `CRUD` action correspond to?

  > | creaste- post, read-post, update-put, delet-delet|

03. What does `ORM` stand for? Which `ORM` do we use when interacting with MongoDB

  > | Object relationship-Model, |

04. Which two `HTTP` request types include a body?

  > | post and put requests|

05. In a/an _______ coding model, when you call a function, it returns only when the action has finished and stops your program for the time the action takes. Likewise in a/an _______ coding model, multiple things are allowed to happen at one time. When you perform an action, your program continues to run.  Fill in the blanks.

  > | synchronouse , asynchronouse |

06. What are the three types of data relationships? Provide an example of each.

  > | one to one like a toture session one instructor one student, on to many like a class one teacher with many students, and many to many like multiple students with multiple teacher for diffrent subjects |

07. What is middleware?

  > | request, response and next they are responsible for different actions like requestin something and getting the response of that request and next is for catching errors if happen. |

08. The ______ pipeline delivers information from the client while the ______ pipeline returns it. Fill in the blanks.

  > | request , response |

09. Demonstrate the pattern that is used to include a request query with the client's `HTTP` request providing the property `tag` and the value `winter`.

  > |
  async function(query){
    const winter = req.query
   } |

10. What is a ***virtual property***?

  > | it is the information we can get from another website so we can aply them in our website |
