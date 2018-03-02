TOPDIR=..\..\..
!include $(TOPDIR)\common.mak

SOURCEDIR = .
OUTDIR = .

.SUFFIXES: .bbg

BGFS = neeleme.bgf neelemeX.bgf iunholyt.bgf xeoneru.bgf xeoneruX.bgf \
       pear.bgf peartree.bgf orange.bgf orangetree.bgf cookie.bgf \
       mmdrat.bgf mfdrat.bgf arrowgold.bgf newshield.bgf newestshield.bgf \
       brm.bgf throwingdaggers.bgf throwknifeproj.bgf icedrag.bgf dicedrag.bgf \
       grd00050.bgf povshldN1.bgf povshldN2.bgf imortalmaskm.bgf \
       redmaskm.bgf redmaskf.bgf imortalmaskf.bgf prism1.bgf \
       brc.bgf brd.bgf brj.bgf brk.bgf brl.bgf mugo.bgf povbeermug.bgf \
       dragonborneheadtest.bgf lavafrog.bgf \
       fbow.bgf \
       fbowaov.bgf \
       fbowbov.bgf \
       fbowinhand.bgf

!include $(RESOURCEDIR)\copy.mak

{$(SOURCEDIR)}.bbg.bgf:
   $(MAKEBGF) -o $(OUTDIR)\$*.bgf @$*.bbg

clean:

