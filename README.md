# Ansible role: FreeBSD Hardening
This role attempts to do simple hardening of a FreeBSD system

# Tasks
## [sysctl](tasks/sysctl.yaml)
Simple sysctl hardening. **NOTE**: Currently doesn't change kern.randompid!
## mac_seeotheruids
Enables the 'see other UIDs' MAC module (see mac_seeotheruids(4))
### Variables
**savagedlight_fbsdharden_mac_seeotheruids**: Enables this task if defined.
**savagedlight_fbsdharden_mac_seeotheruids_gid**: Specifies which group ID will be allowed to see other UIDs processes.