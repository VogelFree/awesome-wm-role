# awesome-wm-role
Ansible role to install awesome window manager

## Install molecule
````bash
pip3 install --user virtualenv
python3 -m virtualenv molecule_ansible
source molecule_ansible/bin/active
pip install -r requirements.txt
```

## Initialize the role with molecule
``` bash
docker run --rm -it \
  -v "$(pwd)":/molecule/ \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -w /molecule/ \
  quay.io/ansible/molecule:3.0.0 \
  molecule init role awesome-window-manager
```
