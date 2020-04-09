
# Magit Apply patches


# Scenario

  - Apply some patches from a file or directory that contains multiple patches.



# Basic Command

  - None



# Workflow

   1. Press `w` inside magit in default buffer or **log view**.

   2. Select patch method.

      2a. Press `w` to apply multiple patches.

        - requires to select a directory.

      2b. Press `a` to apply a single patch.

        - requires to select a file.
        
        - option table

          | option | Description             | Meaning                    |
          | -      | -                       | -                          |
          | `-i`   | Also apply to index     | also apply to staging area |
          | `-c`   | Only apply to index     | only apply to worktree     |
          | `-3`   | Fall back on 3way merge | just like git merge        |


   4. If there's conflict then it will abort patch process unless option is `-3` at stage 2b.



# TODO

   - Actually practice the 2b stage with varying options.
