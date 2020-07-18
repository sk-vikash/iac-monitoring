## Grafana and Prometheus on the AWS
Repo contains script to install grafana and prometheus service onto AWS.

## Technologies Used
```
AWS
Terraform
Bash
VSCode
```

## Prerequite
Create private and public key required in the script by executing the below command.

```
cd Monitoring/
ssh-keygen -f monitoring-key -P ""
```
## Provision

Run below command to provision the infrastructure.

`bash provision.bash 1`

Once infrastructure is created, use following `ip:port` on the browser to open grafana and promethhues
Grafana: instance_public_ip:3000
Prometheus: instance_public_ip:9090

## De-provision

Run below command to de-provision the infrastructure.

`bash provision.bash 0`
