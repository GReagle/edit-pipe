edit-pipe(1)              BSD General Commands Manual             edit-pipe(1)

NNAAMMEE
     eeddiitt--ppiippee — use an editor in a pipeline

SSYYNNOOPPSSIISS
     eeddiitt--ppiippee [--vv]

DDEESSCCRRIIPPTTIIOONN
     The eeddiitt--ppiippee command enables an editor to be used in a pipeline, includ‐
     ing as a pager.  This program was inspired by vipe of moreutils.

OOPPTTIIOONNSS
     --vv      view only, i.e. do not produce output; for the end of a pipeline,
             in order to use editor as a pager

EENNVVIIRROONNMMEENNTT
     The editor is taken from VISUAL if defined, else EDITOR if defined, else
     /usr/bin/editor if there, else /usr/bin/vi if there.

EEXXAAMMPPLLEESS
     ls | eeddiitt--ppiippee | sort -r

     man mv | eeddiitt--ppiippee -v

SSEEEE AALLSSOO
     vipe(1)

BSD                             August 27, 2017                            BSD
