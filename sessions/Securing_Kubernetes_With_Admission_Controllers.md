## Securing Kubernetes With Admission Controllers - Dave Strebel, Microsoft
- by @dave_strebel
#### Admission Contrllers:
- There are default admission controllers
    - NamespaceLifecycle
    - LimitRanger
    - ServiceAccount
    - PVLables
    - DefaultStorageClass

- Admission controllers: def refer k8s.io site
    - Validating webhook
    - Mutating webhook
        - ☝ are dynamic admission controller
    - Policy enforcement
- Home OPA Policy Controller: GitHub :Azure/kubernetes-policy-controller
- OPA policy runs in-memory, so no latency.

- can restrict the exec into containers as well
- Patch the services in admission controller in such a wat not to get out of the network as well. (shown in demo)


- deploy the rego file in the namespace as a configmap

👉🏻 Takeaways -> we can have a admission controller to inject and enforce the labels for deployments.


