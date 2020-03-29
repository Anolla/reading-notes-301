#  jQuery, Events, and The DOM

## selesction in jQuery

- syntax: ${'selector'}.action()

- (selector): finds HTML elements.
the action() is then performed on the element(s).

## Reasons to use jQuery:

1: SIMPLE SELECTORS
2: COMMON TASKS IN LESS CODE
3: CROSS-BROWSER COMPATIBILITY

#### With jQuery, when a selector returns multiple elements, you can update all of them using the one method. There is no need to use a loop.

- **chaining** If you want to use more than one jQuery method on the same selection of elements, you can list several methods at a time using dot notation to separate each one, as shown below.
$( 'l i [i d!="one"] ') . hide() .delay(SOO) . fadeln(1400);

## Getting and updating  content 

- html() and text()

## Inserting new elements

before() , after() , prepend() , append()

## GETTING AND SETTING ATTRIBUTE VALUES

attr() , removeAttr(), addClass(), removeClass()

## GETTING & SETTING CSS PROPERTIES

- SETTING MULTIPLE PROPERTIES: $('1 i ') .css({ ' background- col or' : ' #272727' ,' font-family' : 'Courier'} ) ;

## EVENT METHODS

The on () method is used to handle all events. Behind the scenes, jQuery handles all of the cross-browser issues you saw in the last chapter.


# PAIR PROGRAMMING
* pair programming in a sentense "two brains are better than one"