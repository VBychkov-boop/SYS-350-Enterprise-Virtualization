# Enterprise Build with Terraform
**Student:** Victoria | **Course:** SYS-350

## Project Overview
Single Terraform project deploying Docker containers and KVM VMs on a shared hypervisor, driven entirely by terraform.tfvars.

## Deployed Services
| Service | Network | Port |
|---|---|---|
| Gitea | devops | 4000 |
| Draw.io | devops | 4001 |
| Vaultwarden | internal | 4002 |
| StirlingPDF | internal | 4003 |
| PrivateBin | internal | 4004 |
| MySQL | web | 4006 |
| WordPress | web | 4007 |
| Uptime Kuma | devops | 4008 |
| Portainer | devops | 4009 |

## KVM Virtual Machines
| VM | OS | vCPU | RAM |
|---|---|---|---|
| victoria-win-srv | Windows Server 2025 | 2 | 2GB |
| victoria-ubuntu-srv | Ubuntu 26.04 | 1 | 2GB |

## terraform.tfvars Example (redacted)
student_name = "yourname"
networks = ["devops", "internal", "web"]
corp_octet = 51
