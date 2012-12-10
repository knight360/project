env = Environment()  # Initialize the environment#scons have a built in clean function using -c
env.Program(target = 'ma.o', source = ["ma.c"]) #these build the project
env.Program(target = 'cma.o', source = ["cma.c"])
ma = env.Program(target = 'ma.o', source = ["ma.c"])#these are needed to install
cma = env.Program(target = 'cma.o', source = ["cma.c"])
env.Install(dir = "/usr/local/bin", source = ma) #this is how you create the actual installation targets
env.Install(dir = "/usr/local/bin", source = cma)
