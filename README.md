# Overview
This role installs a webhook notification script at `/usr/local/bin/webhook-notify.sh`
This role requires root permissions. It must be called as root. This needs to be managed at the ansible or playbook level.



# Variables

| Name  | Type | Required | Default Value | Description |
| ----- | ---- | -------- | ------------- | ----------- |
| webhook_notify_type | string | no | `rocketchat` | The target service of the webhook |
| webhook_notify_alternate_dns.enabled | boolean | no | `false` | Use an alternate dns server. Useful when used to notify dns service status. |
| webhook_notify_alternate_dns.nameserver | string | no | `1.1.1.1` | The nameserver to use to query the hostname ip. |

# Automatique Testing

This role is tested using Molecule against:
- Python 3.7, 3.8 and 3.9
- CentOS 7/8/9
- Debian 9/10/11/12
