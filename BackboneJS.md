BackboneJS
==========

#CodeSchool
##The Anatomy of Backbone.js
###Intro
- get your truth out of the DOM
- Capitalize the first letter when defining a Model class
- var TodoItem
- every view element has it's own (el)ement

Server | Data
Data > Model > View > DOM

  var TodoItem = Backbone.Model.extend({});
  var todoItem = new TodoItem(
    {description: 'Pick up'}
  );
  
.get > data out of the model
.set > send in a JSON object
.save > sync with the server

create a view instance
use new

render: function() {

}

