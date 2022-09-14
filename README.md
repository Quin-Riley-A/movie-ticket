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
