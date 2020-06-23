This is customized version of mreferre [Yelb app](https://github.com/mreferre/yelb)

The images are customised to be deployed in OpenShift. The customization is allowing the app to work in OCP as well as showing the UI POD IP address.

Tested on OCP 4.4

## Deployment steps

```
$ git clone https://github.com/mohanadelamin/yelb-os.git
$ cd yelb-os
$ oc new-project yelb
$ oc apply -f yelb.yaml
$ oc expose svc yelb-ui -n yelb
```

App UI:
![UI](https://raw.githubusercontent.com/mohanadelamin/yelb-os/master/images/yelb-os.png)
