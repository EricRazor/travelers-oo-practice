# TRAVELERS, DESTINATIONS AND TICKETS

We're building a travel application! A Traveler has many Destinations through Tickets. A Destination can have many Travelers through Tickets. A Ticket belongs to a Destination and a Traveler.

## Deliverables

Implement all of the methods described below

### `Traveler`

+ `Traveler.all`
  + returns all of the travelers
+ `Traveler#tickets`
  + returns an array of `Ticket` instances associated with this instance of `Traveler`.
+ `Traveler#destinations`
  + returns an array of `Destination` that the `Traveler` is planning on going to.
+ `Traveler#plan_trip(destination)`
  + this method receives a `Destination` instance as its only argument and make plans for the traveler to visit that destination.

### `Ticket`

A `Ticket` object represents that an individual traveler has plans to visit a particular destination.

+ `Ticket.all`
  + returns an array of all `Ticket`s
+ `Ticket#traveler`
  + returns the traveler associated with this `Ticket`
+ `Ticket#destination`
  + returns the destination associated with this `Traveler`

### `Destination`

+ `Destination.all`
  + returns an array of all `Destination`
+ `Destination#tickets`
  + returns an array of all the `Ticket`s to this destination
+ `Destination#travelers`
  + returns an array of all of the `Traveler`s with tickets to visit this destination
+ `Destination.most_popular`
  + returns the instance of `Destination` that has the most travelers
