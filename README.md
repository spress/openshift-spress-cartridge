# OpenShift Spress Cartridge

## How to use this cartridge

### using console tool
* Installing the [OpenShift Client Tools](https://developers.openshift.com/en/managing-client-tools.html) (RHC)
* Create a new application on OpenShift using this command:
``` bash
rhc app create spress http://spress.yosymfony.com/openshift-cartridge/manifest.yml
```
* Ready! you can access to your new site.

## Modify your site

* Clone the repository that is associated with your OpenShift gear to your local machine.
The `www/` folder contains your Spress site.
* Make your changes and send a pull to repository.
* Your OpenShift gear will take care of building your site with your changes.

## License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0).