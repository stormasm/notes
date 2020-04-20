
```
alias py='python3'
alias pip='pip3'
alias pii='pip install .'
```

### On MacOs

Out of the box prior to any python installations

```
py -m site --user-base
yields the following location
/Users/ma/Library/Python/3.7

So the first thing to upgrade is pip
pip install --upgrade pip
```

Then you can go ahead and turn on these environment variables.  Anytime you want to do system level stuff and install in /Users/ma/Library/Python/3.7
you must turn these environment variables back off

```
export PYTHONPATH=/j/tmp49
export PYTHONUSERBASE=/j/tmp49
export PIP_USER=yes
```

To install a github repo simply run this command. The repo must have a setup.py file.

pii
