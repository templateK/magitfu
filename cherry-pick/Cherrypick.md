
# Magit Cherry Pick


# Scenario

  - Take some commits from the other branch(possibly same as the current branch) and <br>
    apply them to the current branch.
  


# Basic Command

  -  checking git commands log performed by magit: press `$` key when there's some error(s).

  -  command `l o`  to enter the **log view** of the other branch.

  -  select commit log(s) with `v` keys on the **log view**.


# Workflow

   1. Enther the other **logv iew** of the branch which the source commits resides in.

   2. Select logs from **log view**.

   2. Press single `A` to enter **cherrick transient state**.

   4. Press `A` to cherry pick and commit or press `a` to cherry pick and stage.

     - this operation takes you out from **log view** of the branch which is owner of source commits.

     - if source commit branch is the same as target branch then what happens?

   5. Deal with the **worktree** state.

      5a. Resolve the **conflicts** and save.

      5b. Just skip the **conflicts**. 
        - continue _will not be possible_ at stage 6.

   6. move cursor to `Cherry-Pick` in the **magit buffer**.
     - there's something wrong if magit won't show the entry. check git command log.

   7. press `A` to _continue_ cherry-picking or press `a` to _abort_ at the magit-mode buffer.

       | key | operation | note                                   |
       | -   | -         |  -                                     |
       | `A` | continue  | carry on cherry pick                   |
       | `a` | abort     | return to previous cherry pick state   |
       | `s` | skip      | omit current commits and continue      |
       | `q` | quit      | revet the whole cherry pick operations |



# TODO

   - Abort and quit operation is still ambiguous. we need to actually practice this workflow.
