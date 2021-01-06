# Docker infra

A daemon with multiple frontends (web/tui/cli…) to control multiple hosts that
run services using containers or VMs.

The multiple hosts would be controlled via Ansible, managed by an inventory.

The services would be based on Docker containers, Docker compose configurations,
or even Vagrant VMs.

The services would be able to define "actions" to perform, such as adding users,
checking for updates, upgrading…

The services would have a way to define how to backup and restore files (would
allow for automatic backups).

Port number override from the service's defaults.

Automatic firewall (iptables/nftables) configuration based on the forwarded ports.

Call service "actions" on webhooks? (regenerate static site on github push to
master, …).

Only requirement, the daemon, probably in a scripting language that is without
much dependencies.

It's kind of like HashiCorp's Terraform in the idea, but self-hosted instead of
cloud based.

Frontend using Beeware for minimum effort, most compatible code?
