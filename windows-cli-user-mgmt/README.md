# overview

Using the 'net' command, it is also possible to manage just about everything about a user account.

View all user accounts currently on a machine by :
```shell
net user
```
## adding a new user 

you can use `net user /add <username> <password>` or you can enter the following where using `*` will then allow a prompt where you can enter the contents of the password
```shell
net user /add user3 *
```

## deleting users
you will not get prompted so be carefull
```shell
net user /delete user3
```

## changing user groups

to add users to the Administrator group
```shell
net localgroup Administrators /add user3
```


