# ce-with-nonce

This Extensions provides content elements to inset js and css. The <script> and <stlye> tags will get nonces, so when using 'nonce-proxy' in csp.yaml for js/css, inserted blocks are CSP conform.

Because of differences in content-blocks we use a different version of this extension to please the content-block structure for TYPO3 v12.

# DDEV for TYPO3 extensions

We use [ddev for typo3 extensions](https://github.com/a-r-m-i-n/ddev-for-typo3-extensions) 

Currently available in ddev is
- TYPO3 12.4 LTS

## Usage

### Start DDEV 

Check out your project, with ``.ddev `` folder in it and perform a

```
ddev start
```

on CLI. This will start the containers, but will not install anything automatically.


### Install TYPO3 environments

This environment offers several DDEV commands, to provision the web container, supporting
the following TYPO3 versions:

```
ddev install-v12
```

When the installation is done, you can access an overview here:

- https://ce-with-nonce.ddev.site/

The TYPO3 installations are available here:

- https://v12.ce-with-nonce.ddev.site/typo3


### Credentials

All versions got the same credentials set:

- Username: ``admin``
- Password: ``Password:Password1!`` (also in install tool)


### TYPO3 CLI / typo3_console

To access TYPO3's CLI tools you can utilize ``ddev exec`` like that:
```
ddev exec v12/vendor/bin/typo3
```

### Remove DDEV project

To remove a DDEV project you can use the following command on CLI
```
ddev delete -Oy
```