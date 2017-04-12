# MAKEFILES-chainsaw
Introducction to makefiles (for ASI/ISA)

## This is a makefile

#### -*-MakeFile-*-

short: client.c; \
cc client.c -o client; \
./client

### lets see how it works

### this is a structure of a basic makefile

target: dependencies
[tab]rule(commands to apply)


### due to errors in linux with tabs you can use this alternative notation

target: dependencies; \
[tab]rule(commands to apply); \
[tab]another_rule(commands to apply); \
