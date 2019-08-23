# DOKS

Welcome to the Github presence for [DigitalOcean's managed Kubernetes Service](https://www.digitalocean.com/products/kubernetes/), or DOKS.

The purpose of this repository is to offer a general platform to users that would like to engage in the development process for DOKS. We encourage everybody to file issues for feature requests and bug reports if a better fit cannot be found across one of the [more specific repositories](#related-repositories) within the DOKS / Kubernetes-on-DO ecosystem. (Don't worry, when in doubt just file an issue here and we'll make sure it gets moved to the right place as needed.)

Note that support-related requests should be directed towards one of the [existing support channels](#support-channels).

## Related Repositories

The following list of repositories enable or help manage Kubernetes clusters on DigitalOcean, including both DOKS and DIY (Do-It-Yourself) flavors.

Please prefer filing an issue in one of them if your feature request or bug report is specifically targetting a particular repository.

- [DigitalOcean Cloud Controller Manager](https://github.com/digitalocean/digitalocean-cloud-controller-manager): The the Kubernetes Cloud Controller Manager implementation for DigitalOcean. Responsible for bootstrapping nodes and integrating DigitalOcean Load Balancers through Service objects (including the [list of supported configuration annotations](https://github.com/digitalocean/digitalocean-cloud-controller-manager/blob/master/docs/controllers/services/annotations.md)).
- [CSI-DigitalOcean](https://github.com/digitalocean/csi-digitalocean): A Container Storage Interface (CSI) Driver for DigitalOcean Block Storage. The CSI plugin allows you to conveniently use DigitalOcean Block Storage on DigitalOcean Kubernetes clusters.
- [doctl](https://github.com/digitalocean/doctl): A command line tool for DigitalOcean services that makes it easy to create, update, and delete DOKS clusters.
- [godo](https://github.com/digitalocean/godo): The official DigitalOcean Go API client to support programmatic access to DOKS.
- [kops](https://github.com/kubernetes/kops): kops helps you create, destroy, upgrade, and maintain Kubernetes clusters from the command line. It comes with initial support for running DIY Kubernetes clusters on DigitalOcean ([tutorial](https://github.com/kubernetes/kops/blob/master/docs/tutorial/digitalocean.md)).
- [Cluster Management API implementation for DigitalOcean](https://github.com/kubernetes-sigs/cluster-api-provider-digitalocean): Supports managing Kubernetes clusters on DigitalOcean through the [Cluster Management API](https://github.com/kubernetes-sigs/cluster-api).
- [Kubernetes autoscaler](https://github.com/kubernetes/autoscaler): Autoscaling-related components for Kubernetes, including support for DigitalOcean DOKS. (Note that new features are first introduced into [our custom fork](https://github.com/digitalocean/autoscaler) before being upstreamed.)
- [ExternalDNS](https://github.com/kubernetes-incubator/external-dns): ExternalDNS synchronizes exposed Kubernetes Services and Ingresses with DNS providers. Provides support for DigitalOcean DNS.

## Support Channels

The following list describes ways to reach out for support with regards to DOKS.

- [DigitalOcean Developer Support](https://www.digitalocean.com/support/): Our central entry page for DigitalOcean developers.
- [DigitalOcean Support form](https://www.digitalocean.com/company/contact/#support): File a support request here if you are a DOKS customer
- [Community Q&A](https://www.digitalocean.com/community/questions/): Reach out to the wider DigitalOcean community to ask for DOKS help, or [browse the Kubernetes-specific content](https://www.digitalocean.com/community/tags/kubernetes?type=questions).
- [DOKS Product Documentation](https://www.digitalocean.com/docs/kubernetes/): Our official documentation. Users may also be interested in the related [Load Balancer](https://www.digitalocean.com/docs/networking/load-balancers/) and [Block Storage Volumes](https://www.digitalocean.com/docs/volumes/) sections that DOKS integrates with.
- [DigitalOcean Tutorials for Kubernetes](https://www.digitalocean.com/community/tutorials/?q=kubernetes): DigitalOcean is known for their outstanding tutorials, which includes Kubernetes.
- [DigitalOcean API Reference for Kubernetes](https://developers.digitalocean.com/documentation/v2/#kubernetes): Our REST API to interact with DOKS.
- [Digitalocean Kubernetes Changelog](https://www.digitalocean.com/docs/kubernetes/changelog/): Stay up to date on what shipped with the latest DOKS releases.
- [DigitalOcean on the Kubernetes Slack team](https://kubernetes.slack.com/messages/digitalocean-k8s): Exchange with the DOKS community and DOKS engineers in the `#digitalocean-k8s` channel on the official Kubernetes Slack team.

## Tools

The following tools may prove helpful to developers.

- [github.com/digitalocean/doks-example](https://github.com/digitalocean/doks-example): Example DigitalOcean Kubernetes workload with service exposed through a DO load-balancer.
- [github.com/digitalocean/clusterlint](https://github.com/digitalocean/clusterlint): A linter to check your live Kubernetes cluster for potential issues and bad practices.
- [github.com/digitalocean/doks-debug](https://github.com/digitalocean/doks-debug): A Docker image with Kubernetes manifests for investigation and troubleshooting.
- [github.com/snormore/doks-examples](https://github.com/snormore/doks-examples): Collection of example applications that have been verified to run on DOKS.
- [github.com/snormore/cilium-portmap](https://github.com/snormore/cilium-portmap): A container enabling hostPort support for Cilium (the CNI used in DOKS). Note that this is not needed on newer DOKS releases anymore.

## License

Copyright 2019 DigitalOcean

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
