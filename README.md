# MAKEFILES-chainsaw
Introducction to makefiles (for ASI/ISA)

## This is a makefile
```
#-*-MakeFile-*-
#first rule 
short: client.c; \
cc client.c -o client; \
./client
```
### lets see how it works

### this the structure of a basic makefile
```
target: dependencies
[tab]<another_rule>
```

### due to errors in linux with tabs you can use this alternative notation 
### this is happens beacuse some text editor replace the [tab] with some [spaces]
```
target: dependencies; \
<rule>; \
<another_rule>; \
```
### Simple  example that take no dependencies and open a new [mate-terminal](for linux mint)
```
#-*-MakeFile-*-
#hello world  
hello:
  mate-terminal 
```

### adding a "PHONY" target....
```
.PHONY:client

client:client.c
    cc client.c -o client
```
