### Bootstrapping AngularJS apps
There are 3 important things that happen during the app bootstrap:
1, The injector that will be used for dependency injection is created.
2, The injector will then create the root scope that will become the context for the model of our application.
3, Angular will then "compile" the DOM starting at the ngApp root element, processing any directives and bindings found along the way.

### View and Template
app/index.html:
'''html
<html ng-app="phonecatApp">
<head>

  <script src="bower_components/angular/angular.js"></script>
  <script src="js/controllers.js"></script>
</head>
<body ng-controller="PhoneListCtrl">

  <ul>
    <li ng-repeat="phone in phones">
      <span>{{phone.name}}</span>
      <p>{{phone.snippet}}</p>
    </li>
  </ul>

</body>
</html>
'''

### Model and Controller


### Scope
The concept of a scope in Angular is crucial. A scope can be seen as the glue which allows the template, model and controller to work together. Angular uses scopes, along with the information contained in the template, data model, and controller, to keep models and views separate, but in sync. Any changes made to the model are reflected in the view; any changes that occur in the view are reflected in the model.
