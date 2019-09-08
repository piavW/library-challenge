<h1>Library Challenge</h1>

<h2>User Stories</h2>

``` DONE
As a Librarian
In order to see which books exist in the library 
We need a list showing the title and author 
```

``` DONE
As a Visitor 
In order to see which books exist in the library 
We need a list showing the title and author 
```

```  DONE
As a Librarian 
In order to check if a book is available
We need a file to show book availability
```

``` DONE
As a Visitor
In order to check if a book is available
We need a be able to search for books by title and author
```

``` #We need a checkout-method, and a person/visitor class or instance-double
As a Visitor
In order to read a book
We need to be able to check-out a book from the library
```

``` #we have set_return_date, we don't have method to change it or add to YAML
As a Librarian
In order to track book check-out and return
We need the return date for the book to be a month from check-out
```

``` #Need to add checked_out_books method list to person/visitor class
As a Visitor 
In order to know which books I checked-out 
I need a list of the books I have in possession
```

```
As a Visitor
In order to return book on time
We need to know the return date
```


Instructions
-------
Read this entire README carefully and follow all instructions.

* Challenge time: this weekend, until Monday 9am
* Feel free to use Google, Stack Overflow, your notes, previously written code, books, etc. but work on your own
* If you refer to or have in whole or partially used the solution of another coach or student, please put a link to that in your README
* If you have a partial solution, **still check in a partial solution to GitHub and create a Pull Request**
* You must submit a Pull Request to this repository with your code by 9.30am Monday morning - before the stand-up


### Tasks
----

* Fork the challenge repo: https://github.com/CraftAcademy/library-challenge
* Run the command `bundle install` in the project directory to ensure you have all the gems
* Write your specs and implementation
* Be smart about using Git: commit and push often. Use feature branches.
* Create a Pull Request as soon as possible
* Read the comments from Hound and fix any issues that the service points out.

### Tips
----

##### Some hints:
  * A Person needs to have a list of books that he currently has in his possession. That list needs to include the return date.
  * The return date can be calculated using the `Date` object. Out of the box, there are methods you can use to add days to the current date.
  * Make use of `doubles` when writing your specs
  * Follow the [naming conventions/standards](https://craftacademy.gitbooks.io/coding-as-a-craft/content/extras/naming_standards.html) for methods and variables

### What we are looking for
----
##### I'm hoping to see that:
* You can take a problem set and write a well tested implementation on your own.
* You understand how to define Ruby Classes and work with objects.
* You understand how classes can interact with each other.
* You know how to make use of arrays, hashes, and associated methods to create dynamic lists.
* You know how to write specs and use them as a blueprint in your development.
* I can track your work by following you commit history - so please commit as soon you are done with a feature or when you have made a test pass.

##### In your Pull Request, I'm hoping to see:
* That you are testing the right thing in the right spec file.
* That all tests passing - green is good!
* High test coverage (above 95% is accepted)
* The code is easy to follow: every class has a clear responsibility, methods are short, code is nicely formatted, etc.
* The `README.md` includes information on how to use your solution with command examples in `irb`. (Feel free to remove this text)


**Happy coding!**


Sources for help

Help from StackOverflow answer regarding other ways to change key values within a yaml-file: https://stackoverflow.com/questions/13948951/update-value-of-key-of-a-yaml-file-in-ruby-on-rails
Explanation being: The showed method will write into yml file. If specified key ("Name") is not present in file, it will write new key value othrwise the existing one will be replaced.
    data = YAML.load_file "path/to/yml_file.yml"
    data["Name"] = ABC
    File.open("path/to/yml_file.yml", 'w') { |f| YAML.dump(data, f) }
It will write into yml file. If specified key ("Name") is not present in file, it will write new key value othrwise the existing one will be replaced.
