## ./pachctl undeploy

Tear down a deployed Pachyderm cluster.

### Synopsis


Tear down a deployed Pachyderm cluster.

```
./pachctl undeploy
```

### Options

```
  -a, --all                
                           Delete everything, including the persistent volumes where metadata
                           is stored.  If your persistent volumes were dynamically provisioned (i.e. if
                           you used the "--dynamic-etcd-nodes" flag), the underlying volumes will be
                           removed, making metadata such repos, commits, pipelines, and jobs
                           unrecoverable. If your persistent volume was manually provisioned (i.e. if
                           you used the "--static-etcd-volume" flag), the underlying volume will not be
                           removed.
      --namespace string   Kubernetes namespace to undeploy Pachyderm from. (default "default")
```

### Options inherited from parent commands

```
      --no-metrics           Don't report user metrics for this command
      --no-port-forwarding   Disable implicit port forwarding
  -v, --verbose              Output verbose logs
```

