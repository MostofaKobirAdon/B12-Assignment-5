# Answers of the Questions of Assignment 5

##### 1. What is the difference between **getElementById ,getElementsByClassName, and querySelector / querySelectorAll**?


##### **Ans :** 

Here are the  difference between the given js methods ➡️  
- GetElementById is a DOM method which provides us the HTML element which has the given id . It is   used to find a specific element.

- GetElementsByClassName is a method of DOM  like getElementById but it gives us an HTML collection of elements which have the given class name .We use it to find some elements specifically .

- On the other hand querySelector is a method which gives us the first HTML element by the given css selector . It can find elements with class , id or even tag name.

- querySelectorAll is same as querySelector, but it provides all elements with the selector in a nodelist.


##### 2. How do you **create and insert a new element into the DOM**?

##### **Ans:**

Here are the steps for creating and inserting a new element in DOM:

- Create an element with a tag name.
- add the element in Dom.
Example ➡️:
``` javascript
    const newDiv = document.createElement('div')

    document.getElementById('my-header').appendChild(newDiv);
```

##### 3. What is **Event Bubbling** and how does it work

##### **Ans:**
When an event happens in an element it reaches to the document step by step in the DOM tree.It is called event bubbling. 

And here is how it works ➡️:

- First the event  happens in an element
- Then it goes to the parent
- Like this it will reach to the document


##### 4. What is **Event Delegation** in JavaScript? Why is it useful?

##### **Ans:**
Event Delegation is a technique where in place of attaching event listener to childs we add only a single event listener to the parent.

usefulness :

- If we have so many child, we have to add event listener to each child . In this case event delegation is helpful.
- It saves memory and time.
- It becomes easy to maintain the code.
- The code looks clear and shorter.


##### 5. What is the difference between **preventDefault() and stopPropagation()** methods?

##### **Ans:**
Here are the difference between **preventDefault()** and 
**stopPropagation()**:

- preventDefault() is a method to prevent the default action of an element in a specific event .But it don't stops the propagation. 
- stopPropagation() is a method to stop the event from going further up or down in DOM tree while bubbling or capturing.
