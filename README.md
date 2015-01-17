# OpenShift Spress Cartridge

This cartridge uses [Spress](http://spress.yosymfony.com) 1.1.0, PHP 5.4 and Spresso as default theme.

## How to use this cartridge

### Using console tool
* Installing the [OpenShift Client Tools](https://developers.openshift.com/en/managing-client-tools.html) (RHC).
* Create a new application on OpenShift using this command:
``` bash
rhc app create spress http://spress.yosymfony.com/openshift-cartridge/manifest.yml
```
* Ready! you can access to your new site.

## Modify your site

* Clone the repository that is associated with your OpenShift gear to your local machine.
* `cd /YOUR-REPOSITORY-FOLDER`
* The `www/` folder contains your Spress site.
* Make your changes and send a pull to repository. You do not need to upload your `_site`
folder that is created by running Spress locally.
* Your OpenShift gear will take care of building your site with your changes.

**Note** that each time you make a pull to repository, your site is builing with `--env=prod` option.
Do not change the values for `host` and `port` variables at `config_prod.yml`.

## License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).