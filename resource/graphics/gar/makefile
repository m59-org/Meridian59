# Makefile for Delerium's graphics. This makefile doesn't build .bbg files
# but will copy .bgfs from any directory listed here.

TOPDIR=..\..\..
!include $(TOPDIR)\common.mak

SOURCEDIR = .
OUTDIR = $(CLIENTRUNDIR)\resource
OUTDIRSUB = ..\$(OUTDIR)

BGFS = igreyinvis.bgf isitting.bgf itransferitem.bgf iexplosion.bgf irift.bgf \
       minorshard.bgf majorshard.bgf whiteshard.bgf greenshard.bgf \
       purplegemshard.bgf chaosgemshard.bgf greygemshard.bgf \
       rubygemshard.bgf glowgemshard.bgf diamondshard.bgf \
       lightningprismhuge.bgf xaerdun.bgf grd19081.bgf \
       iminorlink.bgf grd91000.bgf grd91001.bgf grd91002.bgf ihex1.bgf \
       ihexblue.bgf ihexshock.bgf ihexfire.bgf ihexacid.bgf ihexmagic.bgf \
       ihexweapons.bgf ihexholy.bgf ihexunholy.bgf ihexleeches.bgf ihexbarbs.bgf \
       ihexsap.bgf ihexslow.bgf ihexblackmantle.bgf ihexweaken.bgf \
       ihexfester.bgf ihexexhaustion.bgf ihexbecloud.bgf ihexbestill.bgf \
       ilightningstrike.bgf iflamedash.bgf instillingshard.bgf \
       disturbanceshard.bgf angledfragment.bgf \
       biggerxeo.bgf biggestxeo.bgf biggerxeox.bgf biggestxeox.bgf \
       isquishedlightning.bgf imoderatelink.bgf ilink.bgf \
       imajorlink.bgf imasterlink.bgf ibloodrunes.bgf iunhallowedrunes.bgf \
       nequzonprst.bgf iwodachprst.bgf lucius.bgf vrinna.bgf \
       kerrenor.bgf celegorm.bgf unboundankh.bgf bonkproj.bgf \
       phaxt1.bgf phkxt6.bgf phaxt6.bgf phkxt5.bgf phkxt4.bgf \
       phkxt3.bgf phkxt2.bgf phkxt1.bgf phaxt2.bgf phaxt3.bgf phaxt4.bgf \
       phaxt5.bgf blastfireproj.bgf explosivefrostproj.bgf illwoundsproj.bgf \
       shockingfuryproj.bgf vampdrainproj.bgf holdrings.bgf \
       blindring.bgf majorheartstone.bgf \
       deserttwister.bgf airelementaldead.bgf grd00000.bgf \
       grd00001.bgf mazetotem.bgf grd00002.bgf grd00003.bgf \
       grd00005.bgf dragonbornhead.bgf reliquarypillar.bgf \
       ancientgreaves.bgf ancientarmor.bgf \
       shardfusingpillar.bgf shardshatteringpillar.bgf \
       invistotem.bgf grd00010.bgf \
       grd00101.bgf \
       grd00102.bgf \
       grd00103.bgf \
       icedragonscale.bgf \
       dragonbornmask.bgf \
       dragonbornmaskf.bgf \
       sspsmall.bgf \
       sfpsmall.bgf \
       ishieldrodbuff.bgf \
       idispassion.bgf \
       irecklessheart.bgf \
       dyebottle.bgf \
       iaridaria.bgf \
       ihexsever.bgf \
       deflectimpact.bgf \
       greenblindring.bgf \
       dazzlestar.bgf \
       crystalbeing.bgf \
       burningorb.bgf \
       fburningorb.bgf \
       charmprojectile.bgf \
       bindcircle.bgf \
       maul.bgf \
       maulov.bgf \
       povmaul.bgf \
       flail.bgf \
       flailov.bgf \
       povflail.bgf \
       banditscimitar.bgf \
       povbanditscimitar.bgf \
       banditscimitarov.bgf \
       knighthelm.bgf \
       balta.bgf \
       baltaov.bgf \
       povbalta.bgf \
       runedhelm.bgf \
       spikedhelm.bgf \
       shades.bgf \
       watercentipede.bgf \
       underwatericon.bgf \
       monk.bgf \
       timerminutes.bgf \
       timerseconds.bgf
       

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
