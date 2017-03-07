# Collect Supports

This ansible snippet will login to devices and issue the cl-support command.
Once the CL support command has been executed and a new file is available, the 
script uploads the file back to the ansible server into the destination_directory which is controlled by a variable in the collect_support.yml playbook. By default this will result in the creation of the "collected_cl_supports" directory within the main collect_support directory.

### Using the Playbook


```
$ ansible-playbook ./utility_playbooks/collect_support/collect_support.yml
```

Similarly, there is another matching script that will login to a switch and remove any existing CL support files.

```
$ ansible-playbook ./utility_playbooks/remove_support_files.yml
```

