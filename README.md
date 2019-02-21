# AWS AMI for CSYE 6225

## Team Information

| Name | NEU ID | Email Address |
| --- | --- | --- |
| Feng Huang | 001230993 | huang.fe@husky.neu.edu |
| Meng Tan | 001856443 | tan.men@husky.neu.edu |
| | | |
| | | |

## Validate Template

```
packer validate ubuntu-ami.json
```

## Build AMI

```
packer build \
    -var 'aws_access_key=REDACTED' \
    -var 'aws_secret_key=REDACTED' \
    -var 'aws_region=us-east-1' \
    -var 'subnet_id=REDACTED' \
    ubuntu-ami.json
```
