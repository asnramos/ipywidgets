Jupyter Widgets JupyterLab Extension
====================================

A JupyterLab extension for Jupyter/IPython widgets.  Since JupyterLab is in its
pre-release stage, this package integrating widgets into JupyterLab should also
be considered experimental.

Package Install
---------------

**Prerequisites**
* JupyterLab (see package.json for appropriate version, currently [JupyterLab 0.27.0](https://github.com/jupyterlab/jupyterlab/releases/tag/v0.27.0))


```bash
jupyter labextension install @jupyter-widgets/jupyterlab-manager
```

### Version compatibility

Use the appropriate command from the following list to install JupyterLab
extension, which specifies the appropriate compatible version.

* For JupyterLab 0.30.*, use `jupyter labextension install @jupyter-widgets/jupyterlab-manager@0.31`
* For JupyterLab 0.31rc1, use `jupyter labextension install @jupyter-widgets/jupyterlab-manager@0.32`
* For JupyterLab 0.31rc2, use `jupyter labextension install @jupyter-widgets/jupyterlab-manager@0.33`


Source Build
------------

**Prerequisites**
- [git](http://git-scm.com/)
- [node](http://nodejs.org/)

```bash
git clone https://github.com/jupyter-widgets/ipywidgets.git
cd packages/jupyterlab-manager
npm install
npm run build
jupyter labextension link .
```

**Rebuild**

If you want to pull in changes to Jupyter widgets, run `npm run build` at the ipywidgets repo root to update the version of Jupyter widgets in the node_modules directory and rebuild the JupyterLab extension.