# 0x00. AirBnB clone - The console

## Gerneral Learning Objectives :page_with_curl:

* How to create a Python package
* How to create a command interpreter in Python using the cmd module
* What is Unit testing and how to implement it in a large project
* How to serialize and deserialize a Class
* How to write and read a JSON file
* How to manage datetime
* What is an UUID
* What is *args and how to use it
* What is **kwargs and how to use it
* How to handle named arguments in a function

### Console Commands :computer:

* **create**

Display the number of times a class is created.

```
$ ./console.py
(hbnb) create place
** class doesn't exist **
(hbnb) create city
** class doesn't exist **
(hbnb) create City
90cc423e-0087-4a42-be9b-c050a391cb2f
(hbnb) create Place
3c52e064-d1aa-442b-9f52-be3b67f7af10

```

* **all**

Prints the string representations of all instances of a given class.

```
./console.py
(hbnb) create BaseModel
75e2d665-bafb-4f8b-8792-837f05047e47
(hbnb) create User
152a6ee9-9257-4024-9617-1b407a18bd19
(hbnb) 
(hbnb) all BaseModel
[[BaseModel] (75e2d665-bafb-4f8b-8792-837f05047e47) {'id': '75e2d665-bafb-4f8b-8792-837f05047e47', 'created_at': datetime.datetime(2023, 8, 13, 0, 16, 13, 721765), 'updated_at': datetime.datetime(2023, 8, 13, 0, 16, 13, 721799)}]
```


* **count**

Display the number of times a class is created.

```
$ ./console.py
(hbnb) create place
** class doesn't exist **
(hbnb) create city
** class doesn't exist **
(hbnb) create City
90cc423e-0087-4a42-be9b-c050a391cb2f
(hbnb) create Place
3c52e064-d1aa-442b-9f52-be3b67f7af10
(hbnb) count Place
1
(hbnb) count City
1
```

* **show**

Prints the string representation of a class instance based on a given id.

```
(hbnb) show User 152a6ee9-9257-4024-9617-1b407a18bd19
[User] (152a6ee9-9257-4024-9617-1b407a18bd19) {'id': '152a6ee9-9257-4024-9617-1b407a18bd19', 'created_at': datetime.datetime(2023, 8, 13, 0, 16, 21, 840579), 'updated_at': datetime.datetime(2023, 8, 13, 0, 16, 21, 840614)}
```

* **destroy**

Deletes a class instance based on a given id.

```
$ ./console.py
(hbnb) create State
d2d789cd-7427-4920-aaae-88cbcf8bffe2
(hbnb)
(hbnb) destroy State d2d789cd-7427-4920-aaae-88cbcf8bffe2
```

## Unit testing :straight_ruler:

Unittests for AirBnB project was executed using following command:

```
$ python3 unittest -m discover tests
```

Alternatively, you can specify a single test file to run at a time:

```
$ python3 unittest -m tests/test_console.py
```

## Authors :black_nib:
* **Ugochi Talabi** <https://github.com/Shajoshed20>
* **Iyioluwa Awe** <https://github.com/iyiolakeni>
