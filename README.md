# Overview
This role installs a webhook notification script at `/usr/local/bin/webhook-notify.sh`
This role requires root permissions. It must be called as root. This needs to be managed at the ansible or playbook level.



# Variables

| Name  | Type | Required | Default Value | Description |
| ----- | ---- | -------- | ------------- | ----------- |
| webhook_notify_type | string | no | `rocketchat` | The target service of the webhook |

# Automatique Testing

This role is tested using Molecule against:
- Python 3.7, 3.8 and 3.9
- CentOS 7/8/9
- Debian 9/10/11
