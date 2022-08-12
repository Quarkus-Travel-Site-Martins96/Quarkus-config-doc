# Configuration-Documentation-Travel-Scripts
The Travel simple site documentation and configuration for secrets.
Here the script to create and insert example data inside a empty DB.

The applications are already configured for MySQL DB

## Build secrets
The secrets are included inside the YAML files.

In order to build scripts execute the following commands in a logged in shell:

```shell script
oc create -f db-secrets.yml
```

```shell script
oc create -f mail-secrets.yml
```

```shell script
oc create -f captcha-secrets.yml
```

Now on your Openshift project you will have a new Secret Map usable on build.

## Build configmap
Include configmaps inside your Openahift project, in a logged in shell, run:

```shell script
oc create -f endpoints-config.yml
```

___

# P.S.
**These configuration are not real, the password and key must be changed with some real account configuration**