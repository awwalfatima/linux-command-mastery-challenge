#printenv this command checks the environment variable that are already set, syntax: printenv 
#printenv HOME specifacally checks for home variable environment, syntax: printenv HOME
#echo $VAR this too specifaccly checks the Var variable, syntax; echo $VAR
#export this command is a local variable, which means it is only available in the current shell session, syntax: export the name of the variable = value, i.e export MY_VAR="Hello, nice to meet you"
#unset when you no longer need the variable, the unset command is used to remove it, syntax: unset name of the variable, i.e unset MY_VAR
#env this is similar to printenv, it prints out all environment variables. syntax: env
#source when you set up your permanent variable, in order to apply them immedietly, the source command is used, syntax: source /.profile
#echo $PATH tells you the path to executable program.
#export PATH=$PATH: this command is use to modify your path
#cat /etc/environment this shows the configuration file used for setting environment variables.