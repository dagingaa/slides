##  Two-way data bindings

![Two way data binding](img/two_way_data_binding.png)

<small>Source: http://docs.angularjs.org/guide/databinding</small>

note:
- Two way is different. First, the template is compiled by the browser, and
  produces a live view
- It's called a live view because any change in the model are automatically
  propogated to the view
- The model is single-source of truth for the app state
- Much easier for the developer
- No need to write code to keep everything in sync
- The model is completely unaware of the view
- Gratly simplifies testing
