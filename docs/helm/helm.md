## helm

The Helm package manager for Kubernetes.

### Synopsis


The Kubernetes package manager

To begin working with Helm, run the 'helm init' command:

	$ helm init

This will install Tiller to your running Kubernetes cluster.
It will also set up any necessary local configuration.

Common actions from this point include:

- helm search:    search for charts
- helm fetch:     download a chart to your local directory to view
- helm install:   upload the chart to Kubernetes
- helm list:      list releases of charts

Environment:

  $HELM_HOME          set an alternative location for Helm files. By default, these are stored in \~/.helm  
  $HELM_HOST          set an alternative Tiller host. The format is host:port  
  $HELM_NO_PLUGINS    disable plugins. Set HELM_NO_PLUGINS=1 to disable plugins.  
  $TILLER_NAMESPACE   set an alternative Tiller namespace (default "kube-system")  
  $KUBECONFIG         set an alternative Kubernetes configuration file (default "\~/.kube/config")


### Options

```
      --debug                           enable verbose output
      --home string                     location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string                     address of Tiller. Overrides $HELM_HOST
      --kube-context string             name of the kubeconfig context to use
      --tiller-connection-timeout int   the duration (in seconds) Helm will wait to establish a connection to tiller (default 300)
      --tiller-namespace string         namespace of Tiller (default "kube-system")
```

### SEE ALSO
* [helm completion](helm_completion.md)	 - Generate autocompletions script for the specified shell (bash or zsh)
* [helm create](helm_create.md)	 - create a new chart with the given name
* [helm delete](helm_delete.md)	 - given a release name, delete the release from Kubernetes
* [helm dependency](helm_dependency.md)	 - manage a chart's dependencies
* [helm fetch](helm_fetch.md)	 - download a chart from a repository and (optionally) unpack it in local directory
* [helm get](helm_get.md)	 - download a named release
* [helm history](helm_history.md)	 - fetch release history
* [helm home](helm_home.md)	 - displays the location of HELM_HOME
* [helm init](helm_init.md)	 - initialize Helm on both client and server
* [helm inspect](helm_inspect.md)	 - inspect a chart
* [helm install](helm_install.md)	 - install a chart archive
* [helm lint](helm_lint.md)	 - examines a chart for possible issues
* [helm list](helm_list.md)	 - list releases
* [helm package](helm_package.md)	 - package a chart directory into a chart archive
* [helm plugin](helm_plugin.md)	 - add, list, or remove Helm plugins
* [helm repo](helm_repo.md)	 - add, list, remove, update, and index chart repositories
* [helm reset](helm_reset.md)	 - uninstalls Tiller from a cluster
* [helm rollback](helm_rollback.md)	 - roll back a release to a previous revision
* [helm search](helm_search.md)	 - search for a keyword in charts
* [helm serve](helm_serve.md)	 - start a local http web server
* [helm status](helm_status.md)	 - displays the status of the named release
* [helm template](helm_template.md)	 - locally render templates
* [helm test](helm_test.md)	 - test a release
* [helm upgrade](helm_upgrade.md)	 - upgrade a release
* [helm verify](helm_verify.md)	 - verify that a chart at the given path has been signed and is valid
* [helm version](helm_version.md)	 - print the client/server version information

###### Auto generated by spf13/cobra on 14-Mar-2018
