# CentOS 7 image build

## Install python requirements
```
virtualenv -p /bin/python3 .venv
. .venv/bin/activate
pip install -r requirements.txt
```

## Install ansible required roles
```
ansible-galaxy install -r requirements.yml
```

## Build image
```
packer build --force virtualbox-iso.json
```

