# Milestone.2
# Library Management System In C Programming

## Basic C Programming Structure

### Milestone 2

In this project I'll build a Library Management System (LMS) for a university course in C Programming. This must be done using a videostudio compiler This library management system aim is to show a library management system with C programming basic functions. Inside this code, some things must be applicable; a loop, a preprocessor. The usage of standard inputs(studio.h) and standard outputs(stdout.h).

## Installation

This particular case runs only C programming only. This programming contains the following; 

#### Documentation section

Comprises of a single-line comment (//) and a multi-line comment. These comments or comment cannot be read by the compiler, they are for referencing purposes. They are only useful to the coder or the reader. They in no way affect the compiled text.

#### Link section

This section contains the library files, these library files are also preprocessors as any function starting with a '#' is a preprocessor. But the main reason for this link section, is that the link section is used for reading the coded words. All the library files that are to be included in the program are mentioned in this section. The compiler is thus informed about the library files to be linked with the program.

#### Definition

All the symbolic constants that are to be used in the program are defined here. Define section looks like this (#define). Its main function is for reducing workload.
#### Global Declaration Section

All the variables which are used in more than one function are called global variables and they should be declared before they are used anywhere in the program in this section. Example, int main(), or char or getch etc

#### Main Section

Every C program must have exactly one main function all the statements  in the main section must appear between the opening and the closing brace. It must end with a semicolon. This is an example of an independent function as every coded words in c program will not work without this function.

#### Preprocessor

The preprocessor is a part of the compiler which performs preliminary operations. Any text that starts with a # is a Preprocessor.

#### Standard Input

This can be seen as a device or a function used for taking input from devices, such as; mouse, scanner, keyboard, joystick etc. Its basic function is for giving out commands. A standard input as seen as this (<stdio.h>) with the preprocessor attached to it along with the library files.

#### Standard Output

This can be seen as a device used for giving output to a device, such as a projector, headphones, printers, monitors etc. Unlike standard input, standard output basic function or use, is for receiving commands. Standard Output is seen as this (<stdout>)

## Functional Requirement

This app manages many aspects of a university library system, including cataloging, search, circulation, and waiting list. The interface must be web based, and the server needs to be hosted on the cloud, and accessible from anywhere with Internet connection.

### Users and Authentication

There are two roles of users and librarian and patron.

1. A librarian manages cataloging, and can assist circulation as well.
2. A patron is a customer of the library. He can search for books, borrow and returns books.
3. For simplicity, we allow any user with any email address to be able to create his account using an email as the username, and password of his choice. The user also needs to provide a university ID of 6 digits.
4. Your app must send an email to the user with a verification code. The user needs to use that verification code to complete his account registration. A registered user cannot really use features in the system until his account is verified. A confirmation email must be sent to the user after completion of account verification.
5. For simplicity, we only and automatically register any user with an SJSU email account (@sjsu.edu) to be a librarian.  A librarian cannot be a patron, which means he has to use a different email to register if he needs a patron account as well.
6. No two patrons can have the same university ID, neither can two librarians.

### Cataloging

A librarian must be able to manage the catalog of the books.

7. A book item contains at least the following properties
   1. Author
   2. Title
   3. Issuer
   4. Publisher
   5. Year of publication
   6. Location in the library
   7. Number of copies
   8. Issued book
   9. Coverage image(optional)

8. A librarian must be able to search, add, update, and delete books.
   1. Search capability needs to function as a superset of search features to be described below for patrons.  
   2. The minimal feature to add for search is the capability to search for books created or updated by a particular librarian.  
   3. Update and deletion must be able to work together with search, i.e., a librarian must have the capability to find a book through search, then decide to update/delete it.
   4. A book cannot be deleted if it’s checked out by a patron.
   5. Deleting a book also removes the waiting list for it, if there is any

16. For ease of testing and grading, you need to provide the capability for a librarian to set the current date and time for the app. This way it is easier to test features like due date and waiting lists.  This interface for setting the date and time must be positioned at the top right corner of your main UI pages, and the resulted date and time must be clearly displayed along with the time setting interface as well.

