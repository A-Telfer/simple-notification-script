# PyNotify

Notify yourself when your python script (or other programs) are done.

## Usage
CLI
```
notify send "Complete" "Simulation x has finished"
```

or 

```python
import pynotify
pynotify.send("Complete", "simulation x has finished")
```

it can also pipe output
```
python myscripy.py | notify send "Script Done" --pipe
```

## Setup 

### Create an Email Account to Send From

1. Create a new google account

2. Go into the account `settings > security` then allow `Less secure apps`


### Install 
```
pip install --user pynotify-telfer
```

### Configure

Save the bot information
```
notify sender update --email <bot email> --password <bot password>
```

Add your recipients

```
notify add <your email> 
```
