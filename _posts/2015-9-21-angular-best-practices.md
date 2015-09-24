&: 
Any legal expression is allowed, including an expression which contains a function call. Because of this, & bindings are ideal for binding callback functions to directive behaviors.

Savvy readers may be wondering what the difference is between link and controller. The basic difference is that controller can expose an API, and link functions can interact with controllers using require.

Best Practice: use controller when you want to expose an API to other directives. Otherwise use link.
