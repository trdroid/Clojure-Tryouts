# Functions

### Defining functions

In Clojure, functions are defined using the *defn* macro, the syntax of which is as follows:

```clojure
(defn <function name>
  doc-string?
  metadata attr-map?
  [parameter list*]
  prepost conditions-map?
  body-expressions*)
```

The symbols suffixed with a '?' are optional.

**Underneath the hoods**

The *defn* form 

* expands to a *def* to create a *var* with the name \<function name\> and 
* creates a function with *fn* macro
* points the created \<function name\> var to the function

**Defining a basic function**


