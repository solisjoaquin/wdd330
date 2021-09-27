---
title: "Week 01"
date: "2021-09-18"
---

## Notes of DOING STUFF WITH WEB THINGS

### Rememberinh User's info

In this example, we have a function that get a value from the user and save in the localstorage with an ID.

```
function saveStory(){
    var storyName = document.getElementById(“name_input”).value
    var storyHTML = document.getElementById(“story_editor”).value
    localStorage.setItem(storyName, storyHTML)
}
```

Second line says, “Hey document, get the element who’s id is ‘name_input’. Take what you find inside the input box on the screen, its value, and store what you find in a variable named ‘storyName’.”
‘name_input’ is an input tag into which the user can type a name for the story.
‘story_editor’ is the textarea tag where the user types their story.

**When you want to get the user’s input from any input or text area tag, you use the special word 'value'**

Now for the new bit. Using JavaScript you can store any information you want to use later. Even if your user refreshes the page or goes to some other site and then comes back, anything you’ve saved will still be there. Handy! I’m pretty sure the user wants to
save their story so they can edit it or add to it even if they have left the page. Line 4 is the code that stores the story. It uses something called **'localStorage'**.

Line 4 in English is, “Hey, localStorage, store what’s in the storyHTML variable (box) and label that stored piece of information with what you find in the storyName variable (box).”

JavaScript’s local storage uses what techies call ‘key-value pairs.’ That’s fancy talk for ‘description-stuff pairs.’ If you’ve ever seen an old fashioned phone book you’ve seen this in action. The ‘key’ would be the name of the person and the ‘value’ would be their address and phone number.

#### Store a value

```
localStorage.setItem("lastname", "Smith");
```

### Retrieve a value

```
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

**When you want to show something to a user, you use a section and the special word 'innerHTML'**
