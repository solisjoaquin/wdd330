---
title: "Week 03"
date: "2021-10-01"
---

## Chapter 5

### Object Literals

One way to think about an object is that it’s like a dictionary where you look up a property name and see a value. It's like a database of values.

```
const dictionary = {
    a : {
        ab: 'meaning of the word',
        ac: 'meaning of the word'
    }
}
```

Here is an example of an object that describe Superman

```
const superman = {
    name: 'Superman',
    'real name': 'Clark Kent',
    height: 75,
    weight: 235,
    hero: true,
    villain: false,
    allies: ['Batman','Supergirl','Superboy'],
    fly() {
        return 'Up, up and away!';
    }
};
```

You can create objects with computed properties:

```
const hulk = { name: 'Hulk', ['catch' + 'Phrase']: 'Hulk Smash!' };
```

We can also custom the value with a ternary operator:

```
const captainBritain = { name: 'Captain Britain', hero: bewitched ? false : true };
```

### Check if a method exist

use the `in` operator:

```
'city' in superman;
```

Also you use `hasOwnProperty` method:

```
superman.hasOwnProperty('city');
```

## Chapter 6

## Chapter 7
