# Tilt Extensions

A collection of extensions that you may find useful.

## Usage

To use these extensions you will need to specify this repo and then load the extensions you want to use.

For example, in your **Tiltfile** add the following at the top:

```python
v1alpha1.extension_repo(name='rancher-ext', url='https://github.com/rancher-sandbox/tilt-extensions')
v1alpha1.extension(name='project', repo_name='rancher-ext', repo_path='project')
load('ext://project', 'project_enable')
```

### Example Usage

An example of a project using these extensions is [rancher-turtles](https://github.com/rancher-sandbox/rancher-turtles).

## Acknowledgements

The basis for a lot of these extensions are the Cluster API (CAPI) Tiltfile and **tilt-prepare** utility. The contributors to CAPI have done an amazing job with easing development with their Tilt setup :bow:

You can read the Cluster API documentation related to Tilt [here](https://cluster-api.sigs.k8s.io/developer/tilt.html).
