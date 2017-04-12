# MAKEFILES-chainsaw
Introducction to makefiles (for ASI/ISA)

## This is a makefile

#-*-MakeFile-*-
#first rule 
short: client.c; \
cc client.c -o client; \
./client

### lets see how it works

### this is a structure of a basic makefile

target: dependencies
[tab]rule(commands to apply)


### due to errors in linux with tabs you can use this alternative notation 
### this is happends beacuse some text editor replace the [tab] with some [spaces]

target: dependencies; \
[tab]rule(commands to apply); \
[tab]another_rule(commands to apply); \

### Simple  example that take no dependencies and open a new [mate-terminal](for linux mint)

#-*-MakeFile-*-
#hello world  
hello:
  mate-terminal 

