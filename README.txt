edit-pipe(1)		  BSD General Commands Manual		  edit-pipe(1)

NAME
     edit-pipe -- use an editor in a pipeline

SYNOPSIS
     edit-pipe [-v]

DESCRIPTION
     The edit-pipe command enables an editor to be used in a pipeline, includ-
     ing as a pager.  It depends on mktemp(1) which is available at
     http://www.mktemp.org/ if your system does not already have it.  This
     program was inspired by vipe of moreutils.

OPTIONS
     -v      view only, i.e. do not produce output; for the end of a pipeline,
	     in order to use editor as a pager

ENVIRONMENT
     The editor is taken from VISUAL if defined, else EDITOR if defined, else
     /usr/bin/editor if there, else /usr/bin/vi if there.

EXAMPLES
     ls | edit-pipe | sort -r

     man mv | edit-pipe -v

SEE ALSO
     vipe(1), mktemp(1)

BSD				August 27, 2017 			   BSD
