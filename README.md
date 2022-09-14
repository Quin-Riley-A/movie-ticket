Ticket Prices: 
  Adult Ticket Evening First-Release: $13
  Age:
    Adult = x1.0
    Child = x.75
    Senior = x.50
  Time:
    Matinee = x.8
    Evening = x1.0
  Release:
    First: = x1.0
    Re-release: x.8

So first the user will be presented with a choice of movies,
when they click they are presented a form relevant to that particular selection.
  The form will prompt user for a time from dropdown menu of options
  Second form will ask for quantities of patrons by age range.

Objects:
  Tickets
    this.movie
    this.movietime
    this.ageGroup
    this.price
    Methods (via prototype)
      ticket.isNewRelease(this.movie) 
        checks against array of new releases
        returns price
      ticket.checkAge(pulls from form) 
        returns age group and scales ticket price
      ticket.checkTime(pulls form selection)    
        returns matinee/evening and scales ticket price


//
Movies on screen

user click movie

Hide other movies, show dropdown menu asking for number of tickets and a next button (save movie name as part of order object)

user enters number of tickets and next button (save number of tickets as part of order object)

hide dropdown menu and next button 

show two new dropdown menus asking for how many children and how many seniors, and another next button (subtract number of tickets by children and seniors, save two new varibles as part of order)

hide the dropdown menus and next button

apply protype method that multiplies number of tickets by ticketprice, generates new var totalprice

apply prototype that subtracts number of children * 25% of ticketprice from totalprice
 
apply prototype that subracts numbre of seniors * 50% of ticketprice from totalprice

Show dropdown menu that lists totalprice

**Describe**
movieChoice
*It will return the name of a singly selected movie*
**Code:**
```javascript
movieChoice(button.id);
```
**Expected Output**
"Morbius"