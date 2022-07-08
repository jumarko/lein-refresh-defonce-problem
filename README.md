# lein-refresh-defonce-problem
Problem with defonce and URLStreamHandlerFactory

the issue reported here: https://github.com/jakemcc/test-refresh/issues/84

Run `lein test-refresh` and then try to modify `lein-refresh-defonce-problem.core`, e.g. by changing the existing dummy-add function.
You will see the error:

```
*************** Running tests ***************
:reloading (lein-refresh-defonce-problem.core lein-refresh-defonce-problem.core-test)
:error-while-loading lein-refresh-defonce-problem.core

Error refreshing environment: Syntax error compiling at (lein_refresh_defonce_problem/core.clj:8:1). java.lang.Error: factory already defined
Finished at 07:06:56.085 (run time: 0.377s)

```
