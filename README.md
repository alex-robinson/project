# TEMPLATE working directory

This repository is designed to facilitate the initialization of a new project.

## How to create a new project repository

Fork the repository to a new project.
Note, it is not possible to fork your own repository to yourself. In this case, do the following:

1. Make a new empty repository on Github. Clone it locally.

    ```bash
    git clone https://github.com/<username>/<new-repo>.git
    ```

2. Add original repository as an upstream remote in new repository.
Doing this will allow you to pull in changes from your original repository to your forked repository.

    ```bash
    cd <new-repo>
    git remote add upstream https://github.com/<username>/project.git
    ```

3. Update new repo with all the changes from your original repository using git pull.

    ```bash
    git pull upstream main
    ```

4. Push to update remote.

    ```bash
    git push
    ```

## How to use it

- Fork the repository to a new project.
- Add analysis scripts to `wrk/`.
- Put any input data in `wrk/data`.
- Any generated output can be stored in `wrk/output`.
- Figures can be saved in `wrk/plots`.
