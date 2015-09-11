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
  ...
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
