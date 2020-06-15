# Makefile for Sunnycatt's graphics. This makefile doesn't build .bbg files
# but will copy .bgfs from any directory listed here.

TOPDIR=..\..\..
!include $(TOPDIR)\common.mak

SOURCEDIR = .
OUTDIR = $(CLIENTRUNDIR)\resource
OUTDIRSUB = ..\$(OUTDIR)

BGFS = runebase.bgf \
       oceancrystalbase.bgf \
       runechained.bgf \
       runedeath.bgf \
       runefeather.bgf \
       runefractured.bgf \
       runehammer.bgf \
       runehexed.bgf \
       runejungle.bgf \
       runemountain.bgf \
       runescaled.bgf \
       runesea.bgf \
       runeserpent.bgf \
       runesword.bgf \
       icharminsect.bgf \
       isummonabomination.bgf
       

DIRS = 

all:
   @-for %i in (*.bgf) do @$(CP) %i $(OUTDIR) >nul
   @-for %i in ($(DIRS)) do @if EXIST %i \
      @echo Making in %i & @for %j in (%i\*.bgf) do \
         @$(CP) %j $(OUTDIR) >nul 2>&1

clean:
   @-for %i in (*.bgf) do @if EXIST $(OUTDIR)\%i @del $(OUTDIR)\%i >nul
   @-for %i in ($(DIRS)) do @if EXIST %i \
      @echo Making clean in %i & cd %i & (@for %j in (*.bgf) do \
         @if EXIST $(OUTDIRSUB)\%j @del $(OUTDIRSUB)\%j >nul ) & cd..
