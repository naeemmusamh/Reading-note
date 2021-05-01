# FUNCTIONS, METHODS & OBJECTS

  let's talking about functions
  *The script is placed inside an immediately invoked function expression
  which helps protect the scope of variables*

  function|CREATE HOTEL OBJECT AND WRITE OUT THE OFFER DETAILS
  --------|-----------------------------
  var hotel = {|Create a hotel object
  name: 'Park',|using object literal syntax
  roomRate: 240,|Amount in dollars
  discount : 15,|Percentage discount
  offerPrice: function() {|Wr ite out the hotel name,
  var offerRate = this .roomRate * ((100 - this .discount) I 100);|standard rate,
  return offerRate;|and the special rate
  var hotel Name, roomRate, specialRate;|Declare variables
  hotelName = document .getElementByid('hotelName');|Get elements
  roomRate = document.getElementByid('roomRate');|Get element s
  specialRate = document .getElementByld('specialRate');|Get element s
  hotelName.textContent = hotel .name;|Write hotel name
  roomRate.textContent = '$ ' + hotel . roomRate .toFixed(2) ;|Write room rate
  specialRate .textContent = '$' +hotel .offerPrice();|Write offer pri ce
  -------|--------------------

  # EXAMPLE:

  var hotel = {
  name: 'Park',
  roomRate: 240,
  discount : 15,
  offerPrice: function() {
  var offerRate = this .roomRate * ((100 - this .discount) I 100);
  return offerRate;
  }
  }

  var hotel Name, roomRate, specialRate;
  hotelName = document .getElementByid('hotelName');
  roomRate = document.getElementByid('roomRate');
  specialRate = document .getElementByld('specialRate');
  hotelName.textContent = hotel .name;
  roomRate.textContent = '$ ' + hotel . roomRate .toFixed(2) ;
  specialRate .textContent = '$' +hotel .offerPrice();


# SUMMARY:

  1. Functions allow you to group a set of related statements together that represent a single task.

  2. Functions can take parameters (information J required to do their job) and may return a value.

  3. An object is a series of variables and functions that represent something from the world around you.

  4. In an object, variables are known as properties of the object; functions are known as methods of the object.

  5. Web browsers implement objects that represent both the browser window and the document loaded into the browser
  window.

  6. JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods
  offer functionality that help you write scripts.

  7. Arrays and objects can be used to create complex data sets (and both can contain the other).


  # let's talking about Decision :

  look at this photo

  <img src="../../IMAGE/102/Screenshot 2021-01-28 105629.jpg">

  <img src="IMAGE/102/Screenshot 2021-01-28 102537.jpg">

  <img src="IMAGE/102/Screenshot 2021-01-28 150017.jpg">
