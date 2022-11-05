If terminal says Superuser creation skipped due to not running in a TTY:
```
$ winpty python manage.py createsuperuser
Username (leave blank to use '...'):
```
To be able to run python commands as usual on windows as well what I normally do is appending an alias line to the `~/.profile` file i.e.
```
MINGW64 ~$ cat ~/.profile
alias python='winpty python'
```
After doing so, either source the `~/.profile` file or simply restart the terminal and the initial command `python manage.py createsuperuser` should work as expected!
