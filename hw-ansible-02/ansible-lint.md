lint playbook/site.yml 
WARNING: PATH altered to include /usr/bin
WARNING  Overriding detected file kind 'yaml' with 'playbook' for given positional argument: playbook/site.yml
WARNING  Listing 11 violation(s) that are fatal
yaml: truthy value should be one of [false, true] (truthy)
playbook/site.yml:47

risky-file-permissions: File permissions unset or incorrect
playbook/site.yml:50 Task/Handler: Make dirs

yaml: trailing spaces (trailing-spaces)
playbook/site.yml:67

yaml: truthy value should be one of [false, true] (truthy)
playbook/site.yml:68

yaml: truthy value should be one of [false, true] (truthy)
playbook/site.yml:75

yaml: trailing spaces (trailing-spaces)
playbook/site.yml:76

risky-file-permissions: File permissions unset or incorrect
playbook/site.yml:77 Task/Handler: Copy cfg file

risky-file-permissions: File permissions unset or incorrect
playbook/site.yml:82 Task/Handler: Copy service file

yaml: trailing spaces (trailing-spaces)
playbook/site.yml:93

yaml: trailing spaces (trailing-spaces)
playbook/site.yml:97

yaml: no new line character at the end of file (new-line-at-end-of-file)
playbook/site.yml:100

You can skip specific rules or tags by adding them to your configuration file:    
# .ansible-lint
warn_list:  # or 'skip_list' to silence them completely
  - experimental  # all rules tagged as experimental
  - yaml  # Violations reported by yamllint

Finished with 8 failure(s), 3 warning(s) on 1 files.