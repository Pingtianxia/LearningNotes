# the learning note of makefile

## what do +, - and @ as profixes to recipe lines?
  @ suppresses the normal 'echo' of the command that is executed.(globally with flag -s or --keep-silent)
  - means ignore the exit status of the command that is executed (normally, a non-zero exit status would stop that part of the build).(globally via the -s flag or --ignore-errors)
  + means 'execute this command under <make -n> (when commands are not normally executed). the + notation is a generalization of the mechanism whereby a command containing ${MAKE} or $(MAKE) is executed under <make -n>

##the reason of error: "*** missing separator.  Stop."
	A:the most common cause for that error is that lines are indented with whitespaces instead of tab characters.

