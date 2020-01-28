# tf-updater
Fetches the latest Terraform binary package and installs it under /usr/local/bin

# Example usage
```bash
$ sudo rm /usr/local/bin/terraform

$ get-latest-terraform.sh
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100  3775  100  3775    0     0   7370      0 --:--:-- --:--:-- --:--:--  7373
Installing Terraform 0.12.20 for linux...
--2020-01-28 23:12:02--  https://releases.hashicorp.com/terraform/0.12.20/terraform_0.12.20_linux_amd64.zip
Resolving releases.hashicorp.com (releases.hashicorp.com)... 151.101.53.183, 2a04:4e42:d::439
Connecting to releases.hashicorp.com (releases.hashicorp.com)|151.101.53.183|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 16207833 (15M) [application/zip]
Saving to: ‘terraform_0.12.20_linux_amd64.zip’

terraform_0.12.20_linux_amd64.zip       100%[============================================================================>]  15.46M  36.0MB/s    in 0.4s

2020-01-28 23:12:02 (36.0 MB/s) - ‘terraform_0.12.20_linux_amd64.zip’ saved [16207833/16207833]

Archive:  terraform_0.12.20_linux_amd64.zip
  inflating: /usr/local/bin/terraform

$ which terraform
/usr/local/bin/terraform

$ terraform -v
Terraform v0.12.20
```
