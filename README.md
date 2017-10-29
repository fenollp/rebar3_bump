# rebar3_bump
rebar3 plugin that autoincrements Erlang apps' semver based on API changes

* [bumperl](https://github.com/aerosol/bumperl)
* [relflow](https://github.com/RJ/relflow)


* [How Elm does it](https://github.com/elm-lang/elm-package/blob/master/README.md#version-rules)

~~~
elm-package will bump versions for you, automatically enforcing these rules
Versions are incremented based on how the API changes:
* PATCH - the API is the same, no risk of breaking code
* MINOR - values have been added, existing values are unchanged
* MAJOR - existing values have been changed or removed
~~~

* [How gopkg.in describes it](http://labix.org/gopkg.in)

~~~
The major version should be increased whenever the respective package API is being changed in an incompatible way.

Examples of modifications that DO NEED a major version change are:
* Removing or renaming *any* exposed name (function, method, type, etc)
* Adding, removing or renaming methods in an interface
* Adding a parameter to a function, method, or interface
* Changing the type of a parameter or result in a function, method, or interface
* Changing the number of results in a function, method, or interface
* Some struct changes (see details below)
~~~
