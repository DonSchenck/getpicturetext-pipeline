# openshift-pipelines-workshop
Workshop to demonstrate OpenShift Pipelines (featuring Tekton)

## Link below
https://redhat-developer-demos.github.io/openshift-pipelines-workshop/


`oc create -f workspace.yaml`

`oc create -f apply_manifest_task.yaml`

`oc create -f getpicturetext-pipeline.yaml`

`tkn pipeline start getpicturetext-build-and-deploy -w name=shared-workspace,claimName=source-pvc -p git-url=https://github.com/donschenck/getpicturetext -p IMAGE=image-registry.openshift-image-registry.svc:5000/rhn-engineering-dsch-dev/getpicturetext:latest`

