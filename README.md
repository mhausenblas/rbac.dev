A site dedicated to good practices and tooling around Kubernetes RBAC. Both pull requests and issues are welcome.

For recipes, tips and tricks around RBAC see [recipes.rbac.dev](https://recipes.rbac.dev/).

## Official Kubernetes docs

- [Authorization](https://kubernetes.io/docs/admin/authorization/)
- [Using RBAC Authorization](https://kubernetes.io/docs/reference/access-authn-authz/rbac/)
- [Controlling Access to the Kubernetes API](https://kubernetes.io/docs/reference/access-authn-authz/controlling-access/)
- [Configure Service Accounts for Pods](https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/)

## Talks and articles

- [Effective RBAC](https://www.youtube.com/watch?v=Nw1ymxcLIDI) by Jordan Liggitt
- [Configure RBAC In Your Kubernetes Cluster](https://docs.bitnami.com/kubernetes/how-to/configure-rbac-in-your-kubernetes-cluster/) via Bitnami
- [Using RBAC, Generally Available in Kubernetes v1.8](https://kubernetes.io/blog/2017/10/using-rbac-generally-available-18/) by Eric Chiang
- [On defaults in Kubernetes RBAC](https://dev.to/mhausenblas/on-some-defaults-in-kubernetes-rbac-270l) by Michael Hausenblas
- [Stop using admin credentials in kubectl](https://goglides.com/blog/create-less-privileges-user-in-kubernetes-using-rbac-for-kubectl/) by Balkrishna Pandey
- [Testing Kubernetes RBAC](https://medium.com/yld-engineering-blog/testing-kubernetes-rbac-5e00dc93af8e/) by Tom Gallacher
- [Demystifying RBAC in Kubernetes](https://www.cncf.io/blog/2018/08/01/demystifying-rbac-in-kubernetes/) via CNCF and Bitnami (video)
- [Configuring permissions in Kubernetes with RBAC](https://medium.com/containerum/configuring-permissions-in-kubernetes-with-rbac-a456a9717d5d/) via Containerum
- [Kubernetes Authorization via Open Policy Agent](https://itnext.io/kubernetes-authorization-via-open-policy-agent-a9455d9d5ceb) by Stefan Büringer

## Tooling

### Generators and operators

- [liggitt/audit2rbac](https://github.com/liggitt/audit2rbac): takes a Kubernetes audit log and username as input, and generates RBAC role and binding objects that cover all the API requests made by that user.
- [reactiveops/rbac-manager](https://github.com/reactiveops/rbac-manager): operator that supports declarative configuration for RBAC with new custom resources.

### Interactive queries

- [corneliusweig/rakkess](https://github.com/corneliusweig/rakkess): show an access matrix for server resources.
- [reactiveops/rbac-lookup](https://github.com/reactiveops/rbac-lookup): allows you to easily find Kubernetes roles and cluster roles bound to any user, service account, or group name.
- [sbueringer/kubernetes-rbacq](https://github.com/sbueringer/kubernetes-rbacq): simplifies querying Subjects and Rights specified in Kubernetes through Roles/ClusterRoles and RoleBindings/ClusterRoleBindings.
- [Ladicle/kubectl-bindrole](https://github.com/Ladicle/kubectl-bindrole): finding Kubernetes roles bound to a specified service account, group or user.
- [aquasecurity/kubectl-who-can](https://github.com/aquasecurity/kubectl-who-can): show all the subjects who have permission to perform a given verb on specified resources, for example, find all the subjects who can create pods in a given namespace, or who can delete nodes in the cluster.
- [mhausenblas/rbIAM](https://github.com/mhausenblas/rbIAM/): a unified AWS IAM & Kubernetes RBAC access control exploration tool.

### Visualization

- [jasonrichardsmith/rbac-view](https://github.com/jasonrichardsmith/rbac-view): visualizes RBAC permissions in tabular format in your browser.
- [team-soteria/rback](https://github.com/team-soteria/rback): generates a graph representation (in Graphviz `dot` format) of a Kubernetes cluster's RBAC settings.
