#1. 
Бэкенд был создан

#2. 
```
pugachevvv@debian-vlad:~/Документы/Netology/DevOps/dz_№31$ terraform workspace list
  default
* prod
  stage
```

```
pugachevvv@debian-vlad:~/Документы/Netology/DevOps/dz_№31$ terraform plan

Terraform used the selected providers to generate the following execution plan. Resource actions are indicated with the following symbols:
  + create

Terraform will perform the following actions:

  # yandex_compute_instance.test[0] will be created
  + resource "yandex_compute_instance" "test" {
      + allow_stopping_for_update = true
      + created_at                = (known after apply)
      + folder_id                 = (known after apply)
      + fqdn                      = (known after apply)
      + hostname                  = "test.netology.cloud"
      + id                        = (known after apply)
      + metadata                  = {
          + "ssh-keys" = <<-EOT
                ubuntu:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDMXep2l14LVzM8qadz1bkXgwO4uRMx18J6Acab8fd0/QYF1zkTqJuO6Iz1ulJt2vOW8yLRjrkZC3ljqUWc71XdS9kGL82k3bSZ3AeSMxFa22zc6KmbfXRut2PqWEdvX1bJo52X10TIlE1S07bOr6BNd0/LS+wZ259mAQvlJMxFx03urSuykajwLQ+v9+VWbMrhXzSmUQ4Fha6hZhS/Izifn/wSFjLMQ+f2WArWXbGW2E9geoEi8kjQHtMt7Qi0Uy4bxjihZrC3NSe+YrjZsgdtyRrgSnWpf0EzKcCnAwOUy2F6hKvufLaE0eZlqdZtHanFYjudnC/TSc0N68MhHdvs+hf31lmipNACnTC+rrZz5y46oblfDePtx6KorEoAecyFlERM52xzqmn9PXw9dtu4egEfB1rvcIjRYSjd11LaN3iW4jL1MS7bmgM2mMWIOlQaZQR6jzddyZSQ6dizrzM8oiiY/S2+pSD7R8VdphORj0oPFHkUSIm8eEZnbpyrLHE= pugachevvv@debian-vlad
            EOT
        }
      + name                      = "test-prod-0"
      + network_acceleration_type = "standard"
      + platform_id               = "standard-v1"
      + service_account_id        = (known after apply)
      + status                    = (known after apply)
      + zone                      = "ru-central1-a"

      + boot_disk {
          + auto_delete = true
          + device_name = (known after apply)
          + disk_id     = (known after apply)
          + mode        = (known after apply)

          + initialize_params {
              + block_size  = (known after apply)
              + description = (known after apply)
              + image_id    = "fd80jfslq61mssea4ejn"
              + name        = "root-node01"
              + size        = 40
              + snapshot_id = (known after apply)
              + type        = "network-nvme"
            }
        }

      + network_interface {
          + index              = (known after apply)
          + ip_address         = (known after apply)
          + ipv4               = true
          + ipv6               = (known after apply)
          + ipv6_address       = (known after apply)
          + mac_address        = (known after apply)
          + nat                = true
          + nat_ip_address     = (known after apply)
          + nat_ip_version     = (known after apply)
          + security_group_ids = (known after apply)
          + subnet_id          = (known after apply)
        }

      + placement_policy {
          + placement_group_id = (known after apply)
        }

      + resources {
          + core_fraction = 100
          + cores         = 2
          + memory        = 2
        }

      + scheduling_policy {
          + preemptible = (known after apply)
        }
    }

  # yandex_compute_instance.test[1] will be created
  + resource "yandex_compute_instance" "test" {
      + allow_stopping_for_update = true
      + created_at                = (known after apply)
      + folder_id                 = (known after apply)
      + fqdn                      = (known after apply)
      + hostname                  = "test.netology.cloud"
      + id                        = (known after apply)
      + metadata                  = {
          + "ssh-keys" = <<-EOT
                ubuntu:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDMXep2l14LVzM8qadz1bkXgwO4uRMx18J6Acab8fd0/QYF1zkTqJuO6Iz1ulJt2vOW8yLRjrkZC3ljqUWc71XdS9kGL82k3bSZ3AeSMxFa22zc6KmbfXRut2PqWEdvX1bJo52X10TIlE1S07bOr6BNd0/LS+wZ259mAQvlJMxFx03urSuykajwLQ+v9+VWbMrhXzSmUQ4Fha6hZhS/Izifn/wSFjLMQ+f2WArWXbGW2E9geoEi8kjQHtMt7Qi0Uy4bxjihZrC3NSe+YrjZsgdtyRrgSnWpf0EzKcCnAwOUy2F6hKvufLaE0eZlqdZtHanFYjudnC/TSc0N68MhHdvs+hf31lmipNACnTC+rrZz5y46oblfDePtx6KorEoAecyFlERM52xzqmn9PXw9dtu4egEfB1rvcIjRYSjd11LaN3iW4jL1MS7bmgM2mMWIOlQaZQR6jzddyZSQ6dizrzM8oiiY/S2+pSD7R8VdphORj0oPFHkUSIm8eEZnbpyrLHE= pugachevvv@debian-vlad
            EOT
        }
      + name                      = "test-prod-1"
      + network_acceleration_type = "standard"
      + platform_id               = "standard-v1"
      + service_account_id        = (known after apply)
      + status                    = (known after apply)
      + zone                      = "ru-central1-a"

      + boot_disk {
          + auto_delete = true
          + device_name = (known after apply)
          + disk_id     = (known after apply)
          + mode        = (known after apply)

          + initialize_params {
              + block_size  = (known after apply)
              + description = (known after apply)
              + image_id    = "fd80jfslq61mssea4ejn"
              + name        = "root-node01"
              + size        = 40
              + snapshot_id = (known after apply)
              + type        = "network-nvme"
            }
        }

      + network_interface {
          + index              = (known after apply)
          + ip_address         = (known after apply)
          + ipv4               = true
          + ipv6               = (known after apply)
          + ipv6_address       = (known after apply)
          + mac_address        = (known after apply)
          + nat                = true
          + nat_ip_address     = (known after apply)
          + nat_ip_version     = (known after apply)
          + security_group_ids = (known after apply)
          + subnet_id          = (known after apply)
        }

      + placement_policy {
          + placement_group_id = (known after apply)
        }

      + resources {
          + core_fraction = 100
          + cores         = 2
          + memory        = 2
        }

      + scheduling_policy {
          + preemptible = (known after apply)
        }
    }

  # yandex_compute_instance.test2["prod_vm1"] will be created
  + resource "yandex_compute_instance" "test2" {
      + allow_stopping_for_update = true
      + created_at                = (known after apply)
      + folder_id                 = (known after apply)
      + fqdn                      = (known after apply)
      + hostname                  = "test.netology.cloud"
      + id                        = (known after apply)
      + metadata                  = {
          + "ssh-keys" = <<-EOT
                ubuntu:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDMXep2l14LVzM8qadz1bkXgwO4uRMx18J6Acab8fd0/QYF1zkTqJuO6Iz1ulJt2vOW8yLRjrkZC3ljqUWc71XdS9kGL82k3bSZ3AeSMxFa22zc6KmbfXRut2PqWEdvX1bJo52X10TIlE1S07bOr6BNd0/LS+wZ259mAQvlJMxFx03urSuykajwLQ+v9+VWbMrhXzSmUQ4Fha6hZhS/Izifn/wSFjLMQ+f2WArWXbGW2E9geoEi8kjQHtMt7Qi0Uy4bxjihZrC3NSe+YrjZsgdtyRrgSnWpf0EzKcCnAwOUy2F6hKvufLaE0eZlqdZtHanFYjudnC/TSc0N68MhHdvs+hf31lmipNACnTC+rrZz5y46oblfDePtx6KorEoAecyFlERM52xzqmn9PXw9dtu4egEfB1rvcIjRYSjd11LaN3iW4jL1MS7bmgM2mMWIOlQaZQR6jzddyZSQ6dizrzM8oiiY/S2+pSD7R8VdphORj0oPFHkUSIm8eEZnbpyrLHE= pugachevvv@debian-vlad
            EOT
        }
      + name                      = "test-for-prod_vm1"
      + network_acceleration_type = "standard"
      + platform_id               = "standard-v1"
      + service_account_id        = (known after apply)
      + status                    = (known after apply)
      + zone                      = "ru-central1-a"

      + boot_disk {
          + auto_delete = true
          + device_name = (known after apply)
          + disk_id     = (known after apply)
          + mode        = (known after apply)

          + initialize_params {
              + block_size  = (known after apply)
              + description = (known after apply)
              + image_id    = "fd80jfslq61mssea4ejn"
              + name        = "root-node01"
              + size        = 40
              + snapshot_id = (known after apply)
              + type        = "network-nvme"
            }
        }

      + network_interface {
          + index              = (known after apply)
          + ip_address         = (known after apply)
          + ipv4               = true
          + ipv6               = (known after apply)
          + ipv6_address       = (known after apply)
          + mac_address        = (known after apply)
          + nat                = true
          + nat_ip_address     = (known after apply)
          + nat_ip_version     = (known after apply)
          + security_group_ids = (known after apply)
          + subnet_id          = (known after apply)
        }

      + placement_policy {
          + placement_group_id = (known after apply)
        }

      + resources {
          + core_fraction = 100
          + cores         = 4
          + memory        = 2
        }

      + scheduling_policy {
          + preemptible = (known after apply)
        }
    }

  # yandex_compute_instance.test2["prod_vm2"] will be created
  + resource "yandex_compute_instance" "test2" {
      + allow_stopping_for_update = true
      + created_at                = (known after apply)
      + folder_id                 = (known after apply)
      + fqdn                      = (known after apply)
      + hostname                  = "test.netology.cloud"
      + id                        = (known after apply)
      + metadata                  = {
          + "ssh-keys" = <<-EOT
                ubuntu:ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABgQDMXep2l14LVzM8qadz1bkXgwO4uRMx18J6Acab8fd0/QYF1zkTqJuO6Iz1ulJt2vOW8yLRjrkZC3ljqUWc71XdS9kGL82k3bSZ3AeSMxFa22zc6KmbfXRut2PqWEdvX1bJo52X10TIlE1S07bOr6BNd0/LS+wZ259mAQvlJMxFx03urSuykajwLQ+v9+VWbMrhXzSmUQ4Fha6hZhS/Izifn/wSFjLMQ+f2WArWXbGW2E9geoEi8kjQHtMt7Qi0Uy4bxjihZrC3NSe+YrjZsgdtyRrgSnWpf0EzKcCnAwOUy2F6hKvufLaE0eZlqdZtHanFYjudnC/TSc0N68MhHdvs+hf31lmipNACnTC+rrZz5y46oblfDePtx6KorEoAecyFlERM52xzqmn9PXw9dtu4egEfB1rvcIjRYSjd11LaN3iW4jL1MS7bmgM2mMWIOlQaZQR6jzddyZSQ6dizrzM8oiiY/S2+pSD7R8VdphORj0oPFHkUSIm8eEZnbpyrLHE= pugachevvv@debian-vlad
            EOT
        }
      + name                      = "test-for-prod_vm2"
      + network_acceleration_type = "standard"
      + platform_id               = "standard-v1"
      + service_account_id        = (known after apply)
      + status                    = (known after apply)
      + zone                      = "ru-central1-a"

      + boot_disk {
          + auto_delete = true
          + device_name = (known after apply)
          + disk_id     = (known after apply)
          + mode        = (known after apply)

          + initialize_params {
              + block_size  = (known after apply)
              + description = (known after apply)
              + image_id    = "fd80jfslq61mssea4ejn"
              + name        = "root-node01"
              + size        = 60
              + snapshot_id = (known after apply)
              + type        = "network-nvme"
            }
        }

      + network_interface {
          + index              = (known after apply)
          + ip_address         = (known after apply)
          + ipv4               = true
          + ipv6               = (known after apply)
          + ipv6_address       = (known after apply)
          + mac_address        = (known after apply)
          + nat                = true
          + nat_ip_address     = (known after apply)
          + nat_ip_version     = (known after apply)
          + security_group_ids = (known after apply)
          + subnet_id          = (known after apply)
        }

      + placement_policy {
          + placement_group_id = (known after apply)
        }

      + resources {
          + core_fraction = 100
          + cores         = 8
          + memory        = 2
        }

      + scheduling_policy {
          + preemptible = (known after apply)
        }
    }

  # yandex_vpc_network.network-1 will be created
  + resource "yandex_vpc_network" "network-1" {
      + created_at                = (known after apply)
      + default_security_group_id = (known after apply)
      + folder_id                 = (known after apply)
      + id                        = (known after apply)
      + labels                    = (known after apply)
      + name                      = "network1"
      + subnet_ids                = (known after apply)
    }

  # yandex_vpc_subnet.subnet-1 will be created
  + resource "yandex_vpc_subnet" "subnet-1" {
      + created_at     = (known after apply)
      + folder_id      = (known after apply)
      + id             = (known after apply)
      + labels         = (known after apply)
      + name           = "subnet1"
      + network_id     = (known after apply)
      + v4_cidr_blocks = [
          + "192.168.10.0/24",
        ]
      + v6_cidr_blocks = (known after apply)
      + zone           = "ru-central1-a"
    }

Plan: 6 to add, 0 to change, 0 to destroy.

──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────

Note: You didn't use the -out option to save this plan, so Terraform can't guarantee to take exactly these actions if you run "terraform apply" now.

```
