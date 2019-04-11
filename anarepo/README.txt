directory:

  $TOP/
    README.txt ......... this file

    bin/
      ./anacvsrepo ..... analyze CVS repository
      ./get**** ........ sub tools for anacvsrepo

    CVSROOT.list ....... repository list to analyze

    CVSROOT_0001/
      module.list
      <module_name>/
	.module_co/
        tag.list
	tag.list.sort
	tagsrc.NEWER/   .......... checkout newer files from cvs (cvs co <module>)
	tagsrc.<tag_name>/   ..... export files from cvs (cvs export -r <tag_name>)
	getmodule.log

    CVSROOT_0002/
	:

file format:

     # CVSROOT.list
     n,<CVSROOT_string>
     :

how to use:

    cd $TOP
    # create CVSROOT.list
    ./bin/makecvs

END.
