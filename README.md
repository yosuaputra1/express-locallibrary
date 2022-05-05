# express-locallibrary
This web application creates an online catalog for a small local library, where users can browse available books and manage their accounts.

Created based on https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Tutorial_local_library_website with some changes

# Local Library models

UML association diagram below shows the models we'll define in this case (as boxes). As discussed above, we've created models for the book (the generic details of the book), book instance (status of specific physical copies of the book available in the system), and author. We have also decided to have a model for the genre so that values can be created dynamically. We've decided not to have a model for the BookInstance:status — we will hard code the acceptable values because we don't expect these to change. Within each of the boxes, you can see the model name, the field names and types, and also the methods and their return types.

The diagram also shows the relationships between the models, including their multiplicities. The multiplicities are the numbers on the diagram showing the numbers (maximum and minimum) of each model that may be present in the relationship. For example, the connecting line between the boxes shows that Book and a Genre are related. The numbers close to the Book model show that a Genre must have zero or more Books (as many as you like), while the numbers on the other end of the line next to the Genre show that a book can have zero or more associated Genres.

![locallibrary_models](https://user-images.githubusercontent.com/92204505/166867483-af7b5ae9-5f13-44a7-a5b1-1b6fd4d57eaf.png)

For more information see the associated [MDN tutorial home page](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Tutorial_local_library_website).
