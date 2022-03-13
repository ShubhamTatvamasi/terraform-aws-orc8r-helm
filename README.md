# terraform-aws-orc8r-helm

<!-- BEGIN_TF_DOCS -->
## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_aws"></a> [aws](#requirement\_aws) | >= 2.6.0 |
| <a name="requirement_helm"></a> [helm](#requirement\_helm) | ~> 1.0 |
| <a name="requirement_kubernetes"></a> [kubernetes](#requirement\_kubernetes) | ~> 1.11.1 |
| <a name="requirement_random"></a> [random](#requirement\_random) | ~> 2.1 |
| <a name="requirement_template"></a> [template](#requirement\_template) | ~> 2.0 |
| <a name="requirement_tls"></a> [tls](#requirement\_tls) | ~> 2.1 |

## Providers

| Name | Version |
|------|---------|
| <a name="provider_aws"></a> [aws](#provider\_aws) | >= 2.6.0 |
| <a name="provider_helm"></a> [helm](#provider\_helm) | ~> 1.0 |
| <a name="provider_kubernetes"></a> [kubernetes](#provider\_kubernetes) | ~> 1.11.1 |
| <a name="provider_null"></a> [null](#provider\_null) | n/a |
| <a name="provider_template"></a> [template](#provider\_template) | ~> 2.0 |
| <a name="provider_terraform"></a> [terraform](#provider\_terraform) | n/a |

## Modules

No modules.

## Resources

| Name | Type |
|------|------|
| [aws_iam_access_key.thanos_s3_access_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key) | resource |
| [aws_iam_access_key.yace_access_key](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_access_key) | resource |
| [aws_iam_user.thanos_s3_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user) | resource |
| [aws_iam_user.yace_user](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user) | resource |
| [aws_iam_user_policy.thanos_s3_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy) | resource |
| [aws_iam_user_policy.yace_policy](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/iam_user_policy) | resource |
| [aws_s3_bucket.thanos_object_store_bucket](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/resources/s3_bucket) | resource |
| [helm_release.cert-manager](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.cwf-orc8r](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.dp-orc8r](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.efs_provisioner](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.elasticsearch_curator](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.external_dns](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.feg-orc8r](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.fluentd](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.lte-orc8r](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.orc8r](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.ovpn](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [helm_release.yace_exporter](https://registry.terraform.io/providers/hashicorp/helm/latest/docs/resources/release) | resource |
| [kubernetes_cluster_role_binding.tiller](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/cluster_role_binding) | resource |
| [kubernetes_namespace.monitoring](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/namespace) | resource |
| [kubernetes_namespace.orc8r](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/namespace) | resource |
| [kubernetes_persistent_volume_claim.storage](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/persistent_volume_claim) | resource |
| [kubernetes_secret.artifactory](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.dp_sas_ca](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.dp_sas_certs](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.fluentd_certs](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.nms_certs](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.orc8r_certs](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.orc8r_configs](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_secret.orc8r_envdir](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/secret) | resource |
| [kubernetes_service_account.tiller](https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs/resources/service_account) | resource |
| [null_resource.orc8r_seed_secrets](https://registry.terraform.io/providers/hashicorp/null/latest/docs/resources/resource) | resource |
| [aws_availability_zones.available](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/availability_zones) | data source |
| [aws_eks_cluster.cluster](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/eks_cluster) | data source |
| [aws_eks_cluster_auth.cluster](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/eks_cluster_auth) | data source |
| [aws_iam_policy_document.thanos_s3_policy_doc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_iam_policy_document.yace_policy_doc](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/iam_policy_document) | data source |
| [aws_secretsmanager_secret.orc8r_secrets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/secretsmanager_secret) | data source |
| [aws_secretsmanager_secret_version.orc8r_secrets](https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/secretsmanager_secret_version) | data source |
| [template_file.orc8r_values](https://registry.terraform.io/providers/hashicorp/template/latest/docs/data-sources/file) | data source |
| [terraform_remote_state.current](https://registry.terraform.io/providers/hashicorp/terraform/latest/docs/data-sources/remote_state) | data source |

## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_alertmanager_configurer_version"></a> [alertmanager\_configurer\_version](#input\_alertmanager\_configurer\_version) | Image version for alertmanager configurer. | `string` | `"1.0.4"` | no |
| <a name="input_analytics_app_id"></a> [analytics\_app\_id](#input\_analytics\_app\_id) | App ID for which the metrics is to be exported to | `string` | `""` | no |
| <a name="input_analytics_app_secret"></a> [analytics\_app\_secret](#input\_analytics\_app\_secret) | App secret for which the metrics is to be exported to | `string` | `""` | no |
| <a name="input_analytics_category_name"></a> [analytics\_category\_name](#input\_analytics\_category\_name) | Category under which the exported metrics will be placed under | `string` | `"magma"` | no |
| <a name="input_analytics_export_enabled"></a> [analytics\_export\_enabled](#input\_analytics\_export\_enabled) | Deploy thanos components and object storage | `bool` | `false` | no |
| <a name="input_analytics_metric_export_url"></a> [analytics\_metric\_export\_url](#input\_analytics\_metric\_export\_url) | Metric Export URL | `string` | `""` | no |
| <a name="input_analytics_metrics_prefix"></a> [analytics\_metrics\_prefix](#input\_analytics\_metrics\_prefix) | Bucket name for s3 object storage. Must be globally unique | `string` | `""` | no |
| <a name="input_cert_manager_route53_iam_role_arn"></a> [cert\_manager\_route53\_iam\_role\_arn](#input\_cert\_manager\_route53\_iam\_role\_arn) | IAM role ARN for cert-manager. | `string` | `null` | no |
| <a name="input_cloudwatch_exporter_enabled"></a> [cloudwatch\_exporter\_enabled](#input\_cloudwatch\_exporter\_enabled) | Enable cloudwatch exporter | `bool` | `false` | no |
| <a name="input_cwf_orc8r_chart_version"></a> [cwf\_orc8r\_chart\_version](#input\_cwf\_orc8r\_chart\_version) | Version of the orchestrator cwf module Helm chart to install. | `string` | `"0.2.2"` | no |
| <a name="input_deploy_cert_manager_helm_chart"></a> [deploy\_cert\_manager\_helm\_chart](#input\_deploy\_cert\_manager\_helm\_chart) | Deploy cert-manager helm chart. | `bool` | `false` | no |
| <a name="input_deploy_nms"></a> [deploy\_nms](#input\_deploy\_nms) | Flag to deploy NMS. | `bool` | `true` | no |
| <a name="input_deploy_openvpn"></a> [deploy\_openvpn](#input\_deploy\_openvpn) | Flag to deploy OpenVPN server into cluster. This is useful if you want to remotely access AGWs. | `bool` | `false` | no |
| <a name="input_docker_pass"></a> [docker\_pass](#input\_docker\_pass) | Docker registry password. | `string` | `""` | no |
| <a name="input_docker_registry"></a> [docker\_registry](#input\_docker\_registry) | Docker registry to pull Orchestrator containers from. | `string` | `"docker.artifactory.magmacore.org"` | no |
| <a name="input_docker_user"></a> [docker\_user](#input\_docker\_user) | Docker username to login to registry with. | `string` | `""` | no |
| <a name="input_dp_api_prefix"></a> [dp\_api\_prefix](#input\_dp\_api\_prefix) | Protocol controller api prefix. | `string` | `"/sas/v1"` | no |
| <a name="input_dp_enabled"></a> [dp\_enabled](#input\_dp\_enabled) | Enable domain proxy | `bool` | `false` | no |
| <a name="input_dp_orc8r_chart_version"></a> [dp\_orc8r\_chart\_version](#input\_dp\_orc8r\_chart\_version) | Version of the orchestrator domain proxy module Helm chart to install. | `string` | `"0.1.0"` | no |
| <a name="input_dp_sas_ca"></a> [dp\_sas\_ca](#input\_dp\_sas\_ca) | SAS CA filename. | `string` | `"ca.crt"` | no |
| <a name="input_dp_sas_crt"></a> [dp\_sas\_crt](#input\_dp\_sas\_crt) | SAS certificate filename. | `string` | `"tls.crt"` | no |
| <a name="input_dp_sas_endpoint_url"></a> [dp\_sas\_endpoint\_url](#input\_dp\_sas\_endpoint\_url) | Sas endpoint url where to connect DP to. | `string` | `""` | no |
| <a name="input_dp_sas_key"></a> [dp\_sas\_key](#input\_dp\_sas\_key) | SAS private key filename. | `string` | `"tls.key"` | no |
| <a name="input_efs_file_system_id"></a> [efs\_file\_system\_id](#input\_efs\_file\_system\_id) | ID of the EFS file system to use for K8s persistent volumes. | `string` | n/a | yes |
| <a name="input_efs_provisioner_name"></a> [efs\_provisioner\_name](#input\_efs\_provisioner\_name) | Name of the efs provisioner helm deployment | `string` | `"efs-provisioner"` | no |
| <a name="input_efs_provisioner_role_arn"></a> [efs\_provisioner\_role\_arn](#input\_efs\_provisioner\_role\_arn) | ARN of the IAM role for the EFS provisioner. | `string` | n/a | yes |
| <a name="input_efs_storage_class_name"></a> [efs\_storage\_class\_name](#input\_efs\_storage\_class\_name) | Name of the Storage class | `string` | `"efs"` | no |
| <a name="input_eks_cluster_id"></a> [eks\_cluster\_id](#input\_eks\_cluster\_id) | EKS cluster ID for the K8s cluster. | `string` | n/a | yes |
| <a name="input_elasticsearch_curator_log_level"></a> [elasticsearch\_curator\_log\_level](#input\_elasticsearch\_curator\_log\_level) | Defines Elasticsearch curator logging level. | `string` | `"INFO"` | no |
| <a name="input_elasticsearch_curator_name"></a> [elasticsearch\_curator\_name](#input\_elasticsearch\_curator\_name) | Name of the elasticsearch-curator helm deployment | `string` | `"elasticsearch-curator"` | no |
| <a name="input_elasticsearch_disk_threshold"></a> [elasticsearch\_disk\_threshold](#input\_elasticsearch\_disk\_threshold) | Size threshold in GB. | `number` | `10` | no |
| <a name="input_elasticsearch_endpoint"></a> [elasticsearch\_endpoint](#input\_elasticsearch\_endpoint) | Endpoint of the Elasticsearch datasink for aggregated logs and events. | `string` | `null` | no |
| <a name="input_elasticsearch_port"></a> [elasticsearch\_port](#input\_elasticsearch\_port) | Port Elastic search is listening. | `number` | `443` | no |
| <a name="input_elasticsearch_retention_days"></a> [elasticsearch\_retention\_days](#input\_elasticsearch\_retention\_days) | Retention period in days of Elasticsearch indices. | `number` | `7` | no |
| <a name="input_elasticsearch_use_ssl"></a> [elasticsearch\_use\_ssl](#input\_elasticsearch\_use\_ssl) | Defines if elasicsearch curator should speak to ELK HTTP or HTTPS. | `string` | `"True"` | no |
| <a name="input_existing_tiller_service_account_name"></a> [existing\_tiller\_service\_account\_name](#input\_existing\_tiller\_service\_account\_name) | Name of existing Tiller service account to use for Helm. | `string` | `null` | no |
| <a name="input_external_dns_deployment_name"></a> [external\_dns\_deployment\_name](#input\_external\_dns\_deployment\_name) | Name of the external dns helm deployment | `string` | `"external-dns"` | no |
| <a name="input_external_dns_role_arn"></a> [external\_dns\_role\_arn](#input\_external\_dns\_role\_arn) | IAM role ARN for ExternalDNS. | `string` | n/a | yes |
| <a name="input_feg_orc8r_chart_version"></a> [feg\_orc8r\_chart\_version](#input\_feg\_orc8r\_chart\_version) | Version of the orchestrator feg module Helm chart to install. | `string` | `"0.2.5"` | no |
| <a name="input_fluentd_deployment_name"></a> [fluentd\_deployment\_name](#input\_fluentd\_deployment\_name) | Name of the fluentd helm deployment | `string` | `"fluentd"` | no |
| <a name="input_helm_deployment_name"></a> [helm\_deployment\_name](#input\_helm\_deployment\_name) | Name for the Helm release. | `string` | `"orc8r"` | no |
| <a name="input_helm_pass"></a> [helm\_pass](#input\_helm\_pass) | Helm repository password. | `string` | `""` | no |
| <a name="input_helm_repo"></a> [helm\_repo](#input\_helm\_repo) | Helm repository URL for Orchestrator charts. | `string` | `"https://artifactory.magmacore.org/artifactory/helm/"` | no |
| <a name="input_helm_user"></a> [helm\_user](#input\_helm\_user) | Helm username to login to repository with. | `string` | `""` | no |
| <a name="input_install_tiller"></a> [install\_tiller](#input\_install\_tiller) | Install Tiller in the cluster or not. | `bool` | `true` | no |
| <a name="input_lte_orc8r_chart_version"></a> [lte\_orc8r\_chart\_version](#input\_lte\_orc8r\_chart\_version) | Version of the orchestrator lte module Helm chart to install. | `string` | `"0.2.6"` | no |
| <a name="input_magma_uuid"></a> [magma\_uuid](#input\_magma\_uuid) | UUID to identify Orc8r deployment | `string` | `"default"` | no |
| <a name="input_managed_certs_create"></a> [managed\_certs\_create](#input\_managed\_certs\_create) | This will generate certificates that will be stored in kubernetes secrets. | `bool` | `false` | no |
| <a name="input_managed_certs_enabled"></a> [managed\_certs\_enabled](#input\_managed\_certs\_enabled) | This will enable controller pods to use managed certificates. | `bool` | `false` | no |
| <a name="input_managed_certs_route53_enabled"></a> [managed\_certs\_route53\_enabled](#input\_managed\_certs\_route53\_enabled) | Use Route53 as DNS Provider. | `bool` | `true` | no |
| <a name="input_monitoring_kubernetes_namespace"></a> [monitoring\_kubernetes\_namespace](#input\_monitoring\_kubernetes\_namespace) | K8s namespace to install Orchestrator monitoring components into. | `string` | `"monitoring"` | no |
| <a name="input_nms_custom_issuer"></a> [nms\_custom\_issuer](#input\_nms\_custom\_issuer) | Certificate issuer on Route53 for Let's Encrypt. | `string` | `"orc8r-route53-issuer"` | no |
| <a name="input_nms_managed_certs_enabled"></a> [nms\_managed\_certs\_enabled](#input\_nms\_managed\_certs\_enabled) | This will enable NMS nginx pod to use managed certificate. | `bool` | `false` | no |
| <a name="input_orc8r_chart_version"></a> [orc8r\_chart\_version](#input\_orc8r\_chart\_version) | Version of the core orchestrator Helm chart to install. | `string` | `"1.5.27"` | no |
| <a name="input_orc8r_controller_replicas"></a> [orc8r\_controller\_replicas](#input\_orc8r\_controller\_replicas) | Replica count for Orchestrator controller pods. | `number` | `2` | no |
| <a name="input_orc8r_db_dialect"></a> [orc8r\_db\_dialect](#input\_orc8r\_db\_dialect) | DB dialect for Orchestrator database connection. | `string` | n/a | yes |
| <a name="input_orc8r_db_host"></a> [orc8r\_db\_host](#input\_orc8r\_db\_host) | DB hostname for Orchestrator database connection. | `string` | n/a | yes |
| <a name="input_orc8r_db_name"></a> [orc8r\_db\_name](#input\_orc8r\_db\_name) | DB name for Orchestrator database connection. | `string` | n/a | yes |
| <a name="input_orc8r_db_pass"></a> [orc8r\_db\_pass](#input\_orc8r\_db\_pass) | Orchestrator DB password. | `string` | n/a | yes |
| <a name="input_orc8r_db_port"></a> [orc8r\_db\_port](#input\_orc8r\_db\_port) | DB port for Orchestrator database connection. | `number` | `5432` | no |
| <a name="input_orc8r_db_user"></a> [orc8r\_db\_user](#input\_orc8r\_db\_user) | DB username for Orchestrator database connection. | `string` | n/a | yes |
| <a name="input_orc8r_deployment_type"></a> [orc8r\_deployment\_type](#input\_orc8r\_deployment\_type) | Type of orc8r deployment (fixed wireless access, federated fixed wireless access, or all modules) | `string` | n/a | yes |
| <a name="input_orc8r_domain_name"></a> [orc8r\_domain\_name](#input\_orc8r\_domain\_name) | Base domain name for Orchestrator. | `string` | n/a | yes |
| <a name="input_orc8r_is_staging_deployment"></a> [orc8r\_is\_staging\_deployment](#input\_orc8r\_is\_staging\_deployment) | Indicates if the orc8r-app being deploy is a staging environment.<br>    Staging environment does not deploy Logging, Metrics and Alerts | `bool` | `false` | no |
| <a name="input_orc8r_kubernetes_namespace"></a> [orc8r\_kubernetes\_namespace](#input\_orc8r\_kubernetes\_namespace) | K8s namespace to install main Orchestrator components into. | `string` | `"orc8r"` | no |
| <a name="input_orc8r_proxy_replicas"></a> [orc8r\_proxy\_replicas](#input\_orc8r\_proxy\_replicas) | Replica count for Orchestrator proxy pods. | `number` | `2` | no |
| <a name="input_orc8r_route53_zone_id"></a> [orc8r\_route53\_zone\_id](#input\_orc8r\_route53\_zone\_id) | Route53 zone ID of Orchestrator domain name for ExternalDNS. | `string` | n/a | yes |
| <a name="input_orc8r_tag"></a> [orc8r\_tag](#input\_orc8r\_tag) | Image tag for Orchestrator components. | `string` | `"1.6.1"` | no |
| <a name="input_prometheus_configurer_version"></a> [prometheus\_configurer\_version](#input\_prometheus\_configurer\_version) | Image version for prometheus configurer. | `string` | `"1.0.4"` | no |
| <a name="input_region"></a> [region](#input\_region) | AWS region to deploy Orchestrator components into. The chosen region must provide EKS. | `string` | n/a | yes |
| <a name="input_secretsmanager_orc8r_name"></a> [secretsmanager\_orc8r\_name](#input\_secretsmanager\_orc8r\_name) | Name of the AWS Secrets Manager secret where Orchestrator deployment secrets will be stored. | `string` | n/a | yes |
| <a name="input_seed_certs_dir"></a> [seed\_certs\_dir](#input\_seed\_certs\_dir) | Directory on LOCAL disk where Orchestrator certificates are stored to seed Secrets Manager values. Home directory and env vars will be expanded. | `string` | n/a | yes |
| <a name="input_state_backend"></a> [state\_backend](#input\_state\_backend) | State backend for terraform (e.g. s3, local). | `string` | `"local"` | no |
| <a name="input_state_config"></a> [state\_config](#input\_state\_config) | Optional config for state backend. The object type will depend on your backend. | `any` | `null` | no |
| <a name="input_thanos_compact_node_selector"></a> [thanos\_compact\_node\_selector](#input\_thanos\_compact\_node\_selector) | NodeSelector value to specify which node to run thanos compact pod on. Label is 'compute-type:<value>' | `string` | `""` | no |
| <a name="input_thanos_enabled"></a> [thanos\_enabled](#input\_thanos\_enabled) | Deploy thanos components and object storage | `bool` | `false` | no |
| <a name="input_thanos_object_store_bucket_name"></a> [thanos\_object\_store\_bucket\_name](#input\_thanos\_object\_store\_bucket\_name) | Bucket name for s3 object storage. Must be globally unique | `string` | `""` | no |
| <a name="input_thanos_query_node_selector"></a> [thanos\_query\_node\_selector](#input\_thanos\_query\_node\_selector) | NodeSelector value to specify which node to run thanos query pod on. Default is 'thanos' to be deployed on the default thanos worker group. | `string` | `"thanos"` | no |
| <a name="input_thanos_store_node_selector"></a> [thanos\_store\_node\_selector](#input\_thanos\_store\_node\_selector) | NodeSelector value to specify which node to run thanos store pod on. Label is 'compute-type:<value>' | `string` | `""` | no |
| <a name="input_tiller_namespace"></a> [tiller\_namespace](#input\_tiller\_namespace) | Namespace where Tiller is installed or should be installed into. | `string` | `"kube-system"` | no |
| <a name="input_wifi_orc8r_chart_version"></a> [wifi\_orc8r\_chart\_version](#input\_wifi\_orc8r\_chart\_version) | Version of the orchestrator wifi module Helm chart to install. | `string` | `"0.2.2"` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_helm_vals"></a> [helm\_vals](#output\_helm\_vals) | Helm values for the Orchestrator deployment. |
<!-- END_TF_DOCS -->