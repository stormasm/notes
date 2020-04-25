
```
alias py='python3'
alias pip='pip3'
alias pidot='pip install .'
```

pip is a system level utility and so to upgrade it run
```
sudo pip3 install --upgrade pip
```
when you run in sudo mode you must explicitly type pip3

It will install things run with sudo here:
```
/Library/Python/3.7/site-packages
```

Other system level tools to install off the bat.

```
sudo pip3 install -U pytest
sudo pip3 install -U jupyter

sudo -H pip3 list
```

### On MacOs

Out of the box prior to any python environment installations

```
py -m site --user-base
yields the following location
/Users/ma/Library/Python/3.7
```

Then you can go ahead and turn on these environment variables.    
Anytime you want to install stuff in
```
/Users/ma/Library/Python/3.7
```
you must turn these environment variables back off

```
export PYTHONPATH=/j/tmp49
export PYTHONUSERBASE=/j/tmp49
export PIP_USER=yes
```

To install a github repo simply run this command. The repo must have a setup.py file.

pidot
