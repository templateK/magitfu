
# Magit Cherry Pick


# Basic Command

  -  command `l o`  to enter other branchs **log view**.

  -  select commit log(s) with `v` keys on **log view**.


# Workflow

   1. Enther the other **logv iew** of the branch which the source commits resides in.

   3. Select logs from **log view**.

   2. Press single `A` to enter **cherrick transient state**.

   4. Press `A` to cherry pick and commit or press `a` to cherry pick and stage.

   5. Resolve cherry-picking result.

      a. if there's conflicts, resolve those and save.

      b. move cursor to `Cherry-Pick` entries at the **magit buffer**.

      c. press `A` to _continue_ cherry-picking or press `a` to _abort_ at the magit-mode buffer.

       | key | operation | note                                   |
       | -   | -         |  -                                     |
       | `A` | continue  | carry on cherry pick                   |
       | `a` | abort     | return to previous cherry pick state   |
       | `s` | skip      | omit current commits and continue      |
       | `q` | quit      | revet the whole cherry pick operations |



# TODO

   - Abort and quit operation is still ambiguous. we need to actually practice this workflow.
