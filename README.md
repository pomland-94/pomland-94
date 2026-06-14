# Patrick Omland

**Senior Platform Engineer** — Cloud Native · Enterprise Infrastructure · Operators

I build and operate highly available, secure cloud platforms to modern engineering standards. From OpenStack and Kubernetes infrastructure to the Go operators and SDKs that extend and automate it — I don't just run platforms, I evolve them.

I care about operational correctness over feature velocity: explicit over magic, reproducible over convenient, tested over trusted.

---

## Open Source

### [Contentways/poweradmin-operator](https://github.com/Contentways/poweradmin-operator)
*Kubebuilder · Go · Helm · cosign · SBOM*

DNS lifecycle operator for Kubernetes. Implements `DNSZone` and `DNSRecord` CRDs with per-namespace credential isolation, controller reconciliation loops, envtest-covered test suite, and a production-ready Helm chart with CRD lifecycle hooks. Multi-arch Docker images, SLSA-adjacent supply chain (cosign signatures, SBOM).

### [Contentways/poweradmin-go](https://github.com/Contentways/poweradmin-go)
*Go SDK · Interface-first design*

Full API SDK for Poweradmin — functional options pattern, `IZoneClient`/`IRecordClient` interfaces, generated mocks via gowrap, DTO mapping via goverter. v2 ships string-typed record IDs and DNSSEC support. Follows the hcloud-go design philosophy: no global state, composable, testable.

### [Contentways/poweradmin-cli](https://github.com/Contentways/poweradmin-cli)
*Cobra · Multi-arch*

CLI frontend for the poweradmin-go SDK. Full Poweradmin 4.3.x API coverage, zone export/import, permission templates, auto-generated reference docs, multi-arch Docker.

### [external-dns-poweradmin-webhook](https://github.com/Contentways/external-dns-poweradmin-webhook) *(in progress)*
ExternalDNS webhook provider backed by the poweradmin-go SDK. Brings Poweradmin into the standard Kubernetes DNS automation model.

---



## Engineering Posture

```
Platform  →  Kubernetes · OpenStack · Talos Linux
IaC       →  Terraform · Helm · ArgoCD · Flux
Network   →  OVN/OVS · Octavia · cert-manager · ExternalDNS
Storage   →  Ceph RBD · PostgreSQL/Galera · RabbitMQ
Observ.   →  Prometheus · Grafana · Alertmanager
Auth      →  Keycloak · LDAP · OIDC
Supply    →  cosign/Sigstore · SBOM · Kyverno · GHCR
Dev       →  Go · kubebuilder · Operator SDK · Python · Linux
```
