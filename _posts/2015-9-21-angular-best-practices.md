Controllers should be lightweight and specific to the view they control. A controller should be solely concerned with consuming data, preparing it for the view, and transmitting data to services for processing.

Controllers should be oblivious to the world around them unless you specifically tell them about it. In other words, a controller shouldn’t know about the view it controls and should definitely not know about other controllers.

Services should hold your domain model and do all of the heavy lifting, including server-side communication.

Keep your declarative markup outside of your controllers; conversely, keep your imperative logic outside of your views. It’s really easy to clutter up your view with a complex condition such as ng-if="thisCondition && anotherCondition && yetAnotherCondition". This is hard to maintain and test. Instead, extract that logic structure into a method and bind to that like so: ng-if="shouldShowThis()". This way it is easy to extend shouldShowThis and actually possible to test it.

If you must programmatically manipulate the DOM, then do it in a link function in a directive. This is 99.9% true with a few exceptions, such as a modal service.

Keep your methods fine-grained and as functional (pure) as possible to make testing them easier. This is a general programming principle that’s worth its weight in gold.

Style guides

Todd Motto and John Papa have written excellent style guides that we recommend you check out. These guides are designed to offer helpful suggestions that have worked well for them on large projects; but they suggest you pick what works for you:

Todd Motto’s Style Guide—https://github.com/toddmotto/angularjs-styleguide
John Papa’s Style Guide—https://github.com/johnpapa/angularjs-styleguide

from : Angular in action
