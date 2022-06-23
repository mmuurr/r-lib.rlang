# gghighlight

<details>

* Version: 0.3.3
* GitHub: https://github.com/yutannihilation/gghighlight
* Source code: https://github.com/cran/gghighlight
* Date/Publication: 2022-06-06 20:10:11 UTC
* Number of recursive dependencies: 81

Run `cloud_details(, "gghighlight")` for more info

</details>

## Newly broken

*   checking tests ... ERROR
    ```
      Running ‘testthat.R’
    Running the tests in ‘tests/testthat.R’ failed.
    Last 13 lines of output:
      Backtrace:
          ▆
       1. └─gghighlight:::expect_equal_layers(...) at test-gghighlight.R:260:2
       2.   └─purrr::walk2(x, y, expect_equal_layer) at tests/testthat/helpers.R:14:2
       3.     └─purrr::map2(.x, .y, .f, ...)
       4.       └─gghighlight (local) .f(.x[[i]], .y[[i]], ...)
       5.         └─testthat::expect_equal(as.list(x), as.list(y), ignore_formula_env = TRUE) at tests/testthat/helpers.R:10:2
      
      [ FAIL 38 | WARN 0 | SKIP 1 | PASS 153 ]
      Deleting unused snapshots:
      • vdiffr/simple-bar-chart-with-facet.svg
      • vdiffr/simple-line-chart.svg
      • vdiffr/simple-point-chart.svg
      Error: Test failures
      Execution halted
    ```

# htmltools

<details>

* Version: 0.5.2
* GitHub: https://github.com/rstudio/htmltools
* Source code: https://github.com/cran/htmltools
* Date/Publication: 2021-08-25 13:50:02 UTC
* Number of recursive dependencies: 56

Run `cloud_details(, "htmltools")` for more info

</details>

## Newly broken

*   checking tests ... ERROR
    ```
      Running ‘test-all.R’
    Running the tests in ‘tests/test-all.R’ failed.
    Last 13 lines of output:
      Backtrace:
          ▆
       1. └─htmltools:::expect_equal_tags(z$allTags(), expected) at test-tag-query.R:639:2
       2.   └─testthat::expect_equal(x, y) at tests/testthat/helper-tags.R:23:2
      ── Failure (test-tag-query.R:640:3): tagQuery() objects inherit from each other objects ──
      `x` not equal to `y`.
      Component "children": names for current but not for target
      Backtrace:
          ▆
       1. └─htmltools:::expect_equal_tags(w$allTags(), expected) at test-tag-query.R:640:2
       2.   └─testthat::expect_equal(x, y) at tests/testthat/helper-tags.R:23:2
      
      [ FAIL 4 | WARN 1 | SKIP 5 | PASS 2017 ]
      Error: Test failures
      Execution halted
    ```

## In both

*   checking package dependencies ... NOTE
    ```
    Package which this enhances but not available for checking: ‘knitr’
    ```

# tibble

<details>

* Version: 3.1.7
* GitHub: https://github.com/tidyverse/tibble
* Source code: https://github.com/cran/tibble
* Date/Publication: 2022-05-03 07:00:06 UTC
* Number of recursive dependencies: 101

Run `cloud_details(, "tibble")` for more info

</details>

## Newly broken

*   checking tests ... ERROR
    ```
      Running ‘testthat.R’
    Running the tests in ‘tests/testthat.R’ failed.
    Last 13 lines of output:
           ▆
        1. ├─tibble:::expect_tibble_error(...) at test-tribble.R:124:2
        2. │ └─testthat::expect_error(object, class = class(cnd)[[1]]) at tests/testthat/helper-expectations.R:2:2
        3. │   └─testthat:::expect_condition_matching(...)
        4. │     └─testthat:::quasi_capture(...)
        5. │       ├─testthat (local) .capture(...)
        6. │       │ └─base::withCallingHandlers(...)
        7. │       └─rlang::eval_bare(quo_get_expr(.quo), quo_get_env(.quo))
        8. └─tibble::tribble(~a, ~b, ~c, ~d, 1, 2, 3, 4, 5, 6, 7, 8, 9, )
        9.   └─tibble:::extract_frame_data_from_dots(...)
       10.     └─rlang::cnd_signal(error_tribble_named_after_tilde())
      
      [ FAIL 2 | WARN 0 | SKIP 140 | PASS 1355 ]
      Error: Test failures
      Execution halted
    ```

# tidyquery

<details>

* Version: 0.2.3
* GitHub: https://github.com/ianmcook/tidyquery
* Source code: https://github.com/cran/tidyquery
* Date/Publication: 2021-12-02 20:10:02 UTC
* Number of recursive dependencies: 65

Run `cloud_details(, "tidyquery")` for more info

</details>

## Newly broken

*   checking tests ... ERROR
    ```
      Running ‘testthat.R’
    Running the tests in ‘tests/testthat.R’ failed.
    Last 13 lines of output:
        9. │   └─out %>% ...
       10. ├─tidyquery:::verb(., transmute, !!!(quote_full_expressions(final_select_list)))
       11. │ └─input$data %>% fun(...)
       12. ├─dplyr (local) fun(., ...)
       13. ├─dplyr:::transmute.data.frame(., ...)
       14. │ └─dplyr:::mutate_cols(.data, dots, caller_env = caller_env())
       15. │   ├─base::withCallingHandlers(...)
       16. │   └─mask$eval_all_mutate(quo)
       17. └─base::.handleSimpleError(`<fn>`, "object 'NA' not found", base::quote(mask$eval_all_mutate(quo)))
       18.   └─dplyr (local) h(simpleError(msg, call))
       19.     └─rlang::abort(...)
      
      [ FAIL 1 | WARN 0 | SKIP 2 | PASS 218 ]
      Error: Test failures
      Execution halted
    ```

# WoodSimulatR

<details>

* Version: 0.6.0
* GitHub: NA
* Source code: https://github.com/cran/WoodSimulatR
* Date/Publication: 2022-06-20 06:40:07 UTC
* Number of recursive dependencies: 70

Run `cloud_details(, "WoodSimulatR")` for more info

</details>

## Newly broken

*   checking tests ... ERROR
    ```
      Running ‘testthat.R’
    Running the tests in ‘tests/testthat.R’ failed.
    Last 13 lines of output:
      > library(WoodSimulatR)
      > 
      > test_check("WoodSimulatR")
      [ FAIL 1 | WARN 0 | SKIP 0 | PASS 18 ]
      
      ══ Failed tests ════════════════════════════════════════════════════════════════
      ── Failure (test_statistical_simulation.r:41:3): force_positive works with different simbase classes in simulate_conditionally() ──
      force_positive_works(simbase_class = "simbase_covar", force_positive = TRUE) is not TRUE
      
      `actual`:   FALSE
      `expected`: TRUE 
      
      [ FAIL 1 | WARN 0 | SKIP 0 | PASS 18 ]
      Error: Test failures
      Execution halted
    ```

