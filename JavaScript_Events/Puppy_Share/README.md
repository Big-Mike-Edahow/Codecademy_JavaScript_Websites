Event Object Properties

JavaScript stores events as Event objects with their related data and functionalities as properties and methods. When an event is triggered, the event object can be passed as an argument to the event handler function.

function eventHandlerFunction(event){
   console.log(event.timeStamp);
}

eventTarget.addEventListener('click', eventHandlerFunction);

In the example above, when the 'click' event is triggered on the eventTarget, the eventHandlerFunction receives event, the Event object, which has information related to the 'click' event. Then, we log the time it took for the event to be triggered since the document was loaded by accessing the .timeStamp property of the event object.

There are pre-determined properties associated with event objects. You can call these properties to see information about the event, for example:

The .target property to reference the element that the event is registered to.

The .type property to access the name of the event.

The .timeStamp property to access the number of milliseconds that passed since the document loaded and the event was triggered.
