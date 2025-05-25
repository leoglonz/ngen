# δHBV 2.0 Submodule

---

## About

This submodule is linked in from: <https://github.com/mhpi/dHBV2.0>. This directory follows the template for linking submodules like CFE and LSTM into the NextGen framework.

### Extra Outer Directory

Currently there are two directory layers beneath the top-level *extern/* directory.  This was done so that certain things used by NextGen (i.e., a *CMakeLists.txt* file for building shared library files) can be placed alongside, but not within, the submodule.

## Working with the Submodule

Some simple explanations of several command actions are included below.  To better understand what these things are doing, consult the [Git Submodule documentation](https://git-scm.com/book/en/v2/Git-Tools-Submodules).

### Getting the Latest Changes

There are two steps to getting upstream submodule changes fully:

  1. Fetching and locally checking out the changes from the remote
  2. Committing the new checkout revision for the submodule

To fetch and check out the latest revision:

    ```bash
    git submodule update --init -- ./extern/dhbv2/dhbv2
    ```

To commit the current submodule checkout revision to the MHPI dHBV2.0 MHPI repo:

    ```bash
    git add ./extern/dhbv2/dhbv2
    git commit
    ```
