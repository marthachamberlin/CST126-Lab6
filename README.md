# CST126-Lab6
Oregon Institute of Technology
CST 126 Complex Problem Solving
Lab #6: Linked Lists 1


CST126
Module 6: Lab 6


Linked List
Write the code to create a linked list.
Include the following functionality:
* Insert at the head or tail of the list.
* Delete one or all of the list.
* Print out the linked list.


Create the code to test your linked list.


Inserting code: 20 pts
Deleting code: 20 pts
Printing & Testing code: 10 pts


Submit: full development process


Use the following classes to create your linked list:


List.h
#include "Node.h"
 
class List
{
public:
List();
List(const List& copy);
List& operator = (const List& rhs);
~List();
 
private:
Node* m_head;
};


Node.h
#include "Person.h"
 
class Node
{
public:
Node(Person data);
Person getData();
Node* getNext();
void setData(Person data);
void setNext(Node* next);
private:
Person m_data;
Node* m_next;
};


Person.h
#include <string>;
 
using namespace std;
 
struct Person
{
string first_name;
int age;
char gender;
};
