# Configure Upon Login

After you start using the shell on a regular basis you'll find you enter the same commands each time you login.

The shell with search your `/home` directory for a `.zprofile` file and run the commands that exist in there when you first login. For example, you could setup your `PATH` (aka PASE library list) exactly how you want it.

Use `joe` to edit the file, as shown below.

```
~% joe ~/.zprofile 
```

Add the following content.

```
export PATH=/mydir:$PATH 
echo 'hi mom!' 
```

Save the file and then type `exit` to end the shell session. Go back to the Litmis Spaces dashboard and open a new shell window by selecting the Shell button.

You should see a result like the following: 
``` 
Connecting to Litmis Spaces... 
hi mom 
[usr9q0d8@SPACES]~% 
```

## Please proceed to the next step.
