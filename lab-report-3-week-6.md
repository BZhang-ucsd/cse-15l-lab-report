# Lab Report 3
## Streamlining ssh Configuration

Usually, When we log into ieng6 remote server from your laptop, we will type command line like this:

`$ ssh cs15lwi22xxx@ieng6.ucsd.edu`

However, we can have create a configuration file that shorten the command you have to type.

### Open the Configuration File

Use the command line to open the configuration file:
'~/.ssh/config'
If it does not exits, you can create one.
This command line might not work on windows. You can go to file and open `User/.ssh`

Then create the configuration file `config` in the `.ssh` folder
![1](https://user-images.githubusercontent.com/97600878/153560606-badb21ab-ff12-416c-b2e4-89466e1225f6.png)

In this config file, add：
```
Host ieng6
    HostName ieng6.ucsd.edu
    User cs15lwi22zzz (use your username)
```
You can change your preferred name after `Host`

![WeChat Screenshot_20220211004114](https://user-images.githubusercontent.com/97600878/153560985-19028e35-216c-4ddb-84e4-38b38291d5b0.png)
Then save the file.

### Try SSH Command in Terminal

We can now connect to remote server using shorten command：
`ssh ieng6`
![WeChat Screenshot_20220211004428](https://user-images.githubusercontent.com/97600878/153561358-8828ab6d-c5d4-4cc7-b8da-885727c06eeb.png)
With the ssh key (`id_rsa`) files we create in last tutorial, You should be able to connect to the ieng6 server without typing the course-specific username and password.

You can also use `scp` comman using the shorten named that you set to copy file much faster with shorten command.

![WeChat Screenshot_20220211005613](https://user-images.githubusercontent.com/97600878/153563155-61c0ab6a-30be-4330-b063-ed5cc3106b88.png)


