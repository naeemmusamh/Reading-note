# Event Driven Applications

Event-Driven Programming is a logical pattern that we can choose to confine our programming to avoid complexity and collision issues. Check any major framework or software out there and odds are you’ll find evidence of Event-Driven Programming.


Every time you interact with a webpage through its user interface, an event is happening. When you click a button a click event is triggered. When you press a key down event is triggered. These events have associated functions that, when triggered, are executed to make a change to the user interface in some way.

Event-Driven Programming makes use of the following concepts:

1. An Event Handler is a callback function that will be called when an event is triggered.
2. The Main Loop listens for event triggers and calls the associated event handler for that event.


## EventEmitter


Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challenge, and in fact, there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.



const EventEmitter = require('events').EventEmitter;
const myGatorEvents = new EventEmitter;

class Food {
    constructor(name) {
        this.name = name;
        // Become eaten when gator emits 'gatorEat'
        myGatorEvents.on('gatorEat', this.becomeEaten);
    }

    becomeEaten() {
        return 'I have been eaten.';
    }
}

var bacon = new Food('bacon');

const gator = {
    eat() {
        myGatorEvents.emit('gatorEat');
    }
}

it using with :

1. node.js
2. react
3. game
4. git