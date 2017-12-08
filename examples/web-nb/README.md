# Using jupyter-js-widgets in non-notebook, web context

## Description

This directory is an example project that shows how to use Jupyter widgets in a
web context other than the notebook, but reading and rendering code from a
notebook.

This example requires a Jupyter notebook server to be running. The user is
prompted with a dialog to provide the URL with a running notebook server.

The example is hardcoded to retrieve the `TestNotebook.ipynb` file and execute
code from it.

## Try it

1. Start with a repository checkout, and run `yarn install` in the root directory.
2. Run `yarn run build:examples` in the root directory.
3. Change to this directory
4. Run `yarn run host`
5. In a new terminal run `python -m notebook --no-browser --NotebookApp.allow_origin="*" --NotebookApp.disable_check_xsrf=True --NotebookApp.token=''`. **WARNING: This starts an insecure Jupyter notebook server. Do not do this in production.**
6. In a web browser, navigate to `http://localhost:8080/` (or the address specified by the `yarn run host` command)
