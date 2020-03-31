Virt Tools static site
======================

This directory contains content / configuration for managing

* [https://virttools.org](https://virttools.org)
* [https://virt-tools.org](https://virt-tools.org)
* [https://www.virttools.org](https://www.virttools.org)
* [https://www.virt-tools.org](https://www.virt-tools.org)

The site is setup to run under OpenShift

Initial load can be done with

```
  oc process -f virttools-web/openshift/templates/virttools-web.json  | oc create -f -
```

Updates to the OpenShift config are manually activated using `oc replace`.

Updates to the content itself are automatically propagated via a web hook.
