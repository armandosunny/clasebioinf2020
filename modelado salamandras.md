**###BELLII####**

#########################para recortar las capas con shapes del area de estudio (M)############################

####se cargan los shps con los que se va a cortar las capas#####



`mex=readOGR(".", "belliiprovbien")`
`plot(mex)`


##########PARA RECORTAR LAS CAPAS CREADAS DE LA SERIE6###########################################################################

`Agriculturamaxent=raster("AgriculturamaxentB.asc")`
`AGUAMAXENT=raster("aguamaxentB.asc")`
`ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")`
`ARIDAASCMAXENT=raster("ARIDAASCMAXENB.asc")`
`ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")`
`bio_13=raster("bio_13.asc")`
`bio_14=raster("bio_14.asc")`
`bio_5=raster("bio_5.asc")`
`bio_6=raster("bio_6.asc")`
`BOSQUECULTIVADOASCMAXENT=raster("BOSQUECULTIVADOASCMAXENTB.asc")`
`ENCINOSINHERBASCMAXENTDIST=raster("ENCINOSINHERBASCMAXENTDIST.asc")`
`MESOFILOSINHERBASCMAXENTDIST=raster("MESOFILOSINHERBASCMAXENTDIST.asc")`
`OYAMELASCMAXENTDIST=raster("OYAMELASCMAXENTDIST.asc")`
`PASTIZALINDUCIDOASCMAXENT=raster("PASTIZALINDUCIDOASCMAXENTB.asc")`
`PASTIZALNATURALASCMAXENT=raster("PASTIZALNATURALASCMAXENTB.asc")`
`PASTIZALTODOASCMAXENT=raster("PASTIZALTODOASCMAXENTB.asc")`
`PINOASCMAXENTDIST=raster("PINOASCMAXENTDIST.asc")`
`VEGHIDROFILAASCMAXENT=raster("VEGHIDROFILAASCMAXENTB.asc")`
`SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")`
`SELVACADUCIFOLIAASCMAXENT=raster("SELVACADUCIFOLIAASCMAXENTB.asc")`
`SELVAALTAYBAJAPERENMAXENT=raster("SELVAALTAYBAJAPERENMAXENTB.asc")`
`ENCINOSINHERBASCMAXENTB=raster("ENCINOSINHERBASCMAXENTB.asc")`
`MESOFILOSINHERBASCMAXENTB=raster("MESOFILOSINHERBASCMAXENTB.asc")`
`OYAMELASCMAXENTB=raster("OYAMELASCMAXENTB.asc")`
`PINOASCMAXENTB=raster("PINOASCMAXENTB.asc")`
`pastizalaltamontañaASCS6=raster("pastizalaltamontañaASCS6.asc")`







`mex1=crop(Agriculturamaxent,mex)`
`mex2=crop(AGUAMAXENT,mex)`
`mex3=crop(ALTITUDBIENMAXENT,mex)`
`mex4=crop(ARIDAASCMAXENT,mex)`
`mex5=crop(bio_13,mex)`
`mex6=crop(bio_14,mex)`
`mex7=crop(bio_5,mex)`
`mex8=crop(bio_6,mex)`
`mex9=crop(ASPECTBIENMAXENT,mex)`
`mex10=crop(BOSQUECULTIVADOASCMAXENT,mex)`
`mex11=crop(ENCINOSINHERBASCMAXENTDIST,mex)`
`mex12=crop(MESOFILOSINHERBASCMAXENTDIST,mex)`
`mex13=crop(OYAMELASCMAXENTDIST,mex)`
`mex14=crop(PASTIZALINDUCIDOASCMAXENT,mex)`
`mex15=crop(PASTIZALNATURALASCMAXENT,mex)`
`mex16=crop(PASTIZALTODOASCMAXENT,mex)`
`mex17=crop(PINOASCMAXENTDIST,mex)`
`mex18=crop(VEGHIDROFILAASCMAXENT,mex)`
`mex19=crop(SLOPEBIENMAXENT,mex)`
`mex20=crop(SELVACADUCIFOLIAASCMAXENT,mex)`
`mex21=crop(SELVAALTAYBAJAPERENMAXENT,mex)`
`mex22=crop(ENCINOSINHERBASCMAXENTB,mex)`
`mex23=crop(MESOFILOSINHERBASCMAXENTB,mex)`
`mex24=crop(OYAMELASCMAXENTB,mex)`
`mex25=crop(PINOASCMAXENTB,mex)`
`mex26=crop(pastizalaltamontañaASCS6,mex)`


`mex1b=mask(mex1,mex)`
`mex2b=mask(mex2,mex)`
`mex3b=mask(mex3,mex)`
`mex4b=mask(mex4,mex)`
`mex5b=mask(mex5,mex)`
`mex6b=mask(mex6,mex)`
`mex7b=mask(mex7,mex)`
`mex8b=mask(mex8,mex)`
`mex9b=mask(mex9,mex)`
`mex10b=mask(mex10,mex)`
`mex11b=mask(mex11,mex)`
`mex12b=mask(mex12,mex)`
`mex13b=mask(mex13,mex)`
`mex14b=mask(mex14,mex)`
`mex15b=mask(mex15,mex)`
`mex16b=mask(mex16,mex)`
`mex17b=mask(mex17,mex)`
`mex18b=mask(mex18,mex)`
`mex19b=mask(mex19,mex)`
`mex20b=mask(mex20,mex)`
`mex21b=mask(mex21,mex)`
`mex22b=mask(mex22,mex)`
`mex23b=mask(mex23,mex)`
`mex24b=mask(mex24,mex)`
`mex25b=mask(mex25,mex)`
`mex26b=mask(mex26,mex)`



`writeRaster(mex1b, "Agriculturabellii16.asc")`
`writeRaster(mex2b, "AGUAbellii16.asc")`
`writeRaster(mex3b, "ALTITUDbellii16.asc")`
`writeRaster(mex4b, "ARIDAbellii16.asc")`
`writeRaster(mex5b, "bio_13bellii16.asc")`
`writeRaster(mex6b, "bio_14bellii16.asc")`
`writeRaster(mex7b, "bio_5bellii16.asc")`
`writeRaster(mex8b, "bio_6bellii16.asc")`
`writeRaster(mex9b, "ASPECTbellii16.asc")`
`writeRaster(mex10b, "BOSQUECULTIVADObellii16.asc")`
`writeRaster(mex11b, "ENCINOSINHERBdistbellii16.asc")`
`writeRaster(mex12b, "MESOFILOSINHERBdisbellii16.asc")`
`writeRaster(mex13b, "OYAMELdistbellii16.asc")`
`writeRaster(mex14b, "PASTIZALINDUCIDObellii16.asc")`
`writeRaster(mex15b, "PASTIZALNATURbellii16.asc")`
`writeRaster(mex16b, "PASTIZALTODObellii16.asc")`
`writeRaster(mex17b, "PINOdistbellii16.asc")`
`writeRaster(mex18b, "VEGHIDROFILAbellii16.asc")`
`writeRaster(mex19b, "SLOPEbellii16.asc")`
`writeRaster(mex20b, "SELVACADUCIFOLIAbellii16.asc")`
`writeRaster(mex21b, "SELVAALTAYBAJAPERbellii16.asc")`
`writeRaster(mex22b, "ENCINOSINHERBASbellii16.asc")`
`writeRaster(mex23b, "MESOFILOSINHERBbellii16.asc")`
`writeRaster(mex24b, "OYAMELbellii16.asc")`
`writeRaster(mex25b, "PINObellii16.asc")`
`writeRaster(mex26b, "pastizalaltamontañabellii16.asc")`




###cephalica####

#########################para recortar las capas con shapes del area de estudio (M)############################

####se cargan los shps con los que se va a cortar las capas#####



mex=readOGR(".", "cephalicaprov")
plot(mex)


##########PARA RECORTAR LAS CAPAS CREADAS DE LA SERIE6###########################################################################

Agriculturamaxent=raster("AgriculturamaxentB.asc")
AGUAMAXENT=raster("aguamaxentB.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
ARIDAASCMAXENT=raster("ARIDAASCMAXENB.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio_13=raster("bio_13.asc")
bio_14=raster("bio_14.asc")
bio_5=raster("bio_5.asc")
bio_6=raster("bio_6.asc")
BOSQUECULTIVADOASCMAXENT=raster("BOSQUECULTIVADOASCMAXENTB.asc")
ENCINOSINHERBASCMAXENTDIST=raster("ENCINOSINHERBASCMAXENTDIST.asc")
MESOFILOSINHERBASCMAXENTDIST=raster("MESOFILOSINHERBASCMAXENTDIST.asc")
OYAMELASCMAXENTDIST=raster("OYAMELASCMAXENTDIST.asc")
PASTIZALINDUCIDOASCMAXENT=raster("PASTIZALINDUCIDOASCMAXENTB.asc")
PASTIZALNATURALASCMAXENT=raster("PASTIZALNATURALASCMAXENTB.asc")
PASTIZALTODOASCMAXENT=raster("PASTIZALTODOASCMAXENTB.asc")
PINOASCMAXENTDIST=raster("PINOASCMAXENTDIST.asc")
VEGHIDROFILAASCMAXENT=raster("VEGHIDROFILAASCMAXENTB.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
SELVACADUCIFOLIAASCMAXENT=raster("SELVACADUCIFOLIAASCMAXENTB.asc")
SELVAALTAYBAJAPERENMAXENT=raster("SELVAALTAYBAJAPERENMAXENTB.asc")
ENCINOSINHERBASCMAXENTB=raster("ENCINOSINHERBASCMAXENTB.asc")
MESOFILOSINHERBASCMAXENTB=raster("MESOFILOSINHERBASCMAXENTB.asc")
OYAMELASCMAXENTB=raster("OYAMELASCMAXENTB.asc")
PINOASCMAXENTB=raster("PINOASCMAXENTB.asc")
pastizalaltamontañaASCS6=raster("pastizalaltamontañaASCS6.asc")






mex1=crop(Agriculturamaxent,mex)
mex2=crop(AGUAMAXENT,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(ARIDAASCMAXENT,mex)
mex5=crop(bio_13,mex)
mex6=crop(bio_14,mex)
mex7=crop(bio_5,mex)
mex8=crop(bio_6,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex10=crop(BOSQUECULTIVADOASCMAXENT,mex)
mex11=crop(ENCINOSINHERBASCMAXENTDIST,mex)
mex12=crop(MESOFILOSINHERBASCMAXENTDIST,mex)
mex13=crop(OYAMELASCMAXENTDIST,mex)
mex14=crop(PASTIZALINDUCIDOASCMAXENT,mex)
mex15=crop(PASTIZALNATURALASCMAXENT,mex)
mex16=crop(PASTIZALTODOASCMAXENT,mex)
mex17=crop(PINOASCMAXENTDIST,mex)
mex18=crop(VEGHIDROFILAASCMAXENT,mex)
mex19=crop(SLOPEBIENMAXENT,mex)
mex20=crop(SELVACADUCIFOLIAASCMAXENT,mex)
mex21=crop(SELVAALTAYBAJAPERENMAXENT,mex)
mex22=crop(ENCINOSINHERBASCMAXENTB,mex)
mex23=crop(MESOFILOSINHERBASCMAXENTB,mex)
mex24=crop(OYAMELASCMAXENTB,mex)
mex25=crop(PINOASCMAXENTB,mex)
mex26=crop(pastizalaltamontañaASCS6,mex)


mex1b=mask(mex1,mex)
mex2b=mask(mex2,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex10b=mask(mex10,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex18b=mask(mex18,mex)
mex19b=mask(mex19,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)
mex26b=mask(mex26,mex)



writeRaster(mex1b, "Agriculturacephalica16.asc")
writeRaster(mex2b, "AGUAcephalica16.asc")
writeRaster(mex3b, "ALTITUDcephalica16.asc")
writeRaster(mex4b, "ARIDAcephalica16.asc")
writeRaster(mex5b, "bio_13cephalica16.asc")
writeRaster(mex6b, "bio_14cephalica16.asc")
writeRaster(mex7b, "bio_5cephalica16.asc")
writeRaster(mex8b, "bio_6cephalica16.asc")
writeRaster(mex9b, "ASPECTcephalica16.asc")
writeRaster(mex10b, "BOSQUECULTIVADOcephalica16.asc")
writeRaster(mex11b, "ENCINOSINHERBdistcephalica16.asc")
writeRaster(mex12b, "MESOFILOSINHERBdiscephalica16.asc")
writeRaster(mex13b, "OYAMELdistcephalica16.asc")
writeRaster(mex14b, "PASTIZALINDUCIDOcephalica16.asc")
writeRaster(mex15b, "PASTIZALNATURcephalica16.asc")
writeRaster(mex16b, "PASTIZALTODOcephalica16.asc")
writeRaster(mex17b, "PINOdistcephalica16.asc")
writeRaster(mex18b, "VEGHIDROFILAcephalica16.asc")
writeRaster(mex19b, "SLOPEcephalica16.asc")
writeRaster(mex20b, "SELVACADUCIFOLIAcephalica16.asc")
writeRaster(mex21b, "SELVAALTAYBAJAPERcephalica16.asc")
writeRaster(mex22b, "ENCINOSINHERBAScephalica16.asc")
writeRaster(mex23b, "MESOFILOSINHERBcephalica16.asc")
writeRaster(mex24b, "OYAMELcephalica16.asc")
writeRaster(mex25b, "PINOcephalica16.asc")
writeRaster(mex26b, "pastizalaltamontañacephalica16.asc")



###leprosa####

#########################para recortar las capas con shapes del area de estudio (M)############################

####se cargan los shps con los que se va a cortar las capas#####



mex=readOGR(".", "leprosaprov")
plot(mex)


##########PARA RECORTAR LAS CAPAS CREADAS DE LA SERIE6###########################################################################

Agriculturamaxent=raster("AgriculturamaxentB.asc")
AGUAMAXENT=raster("aguamaxentB.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
ARIDAASCMAXENT=raster("ARIDAASCMAXENB.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio_13=raster("bio_13.asc")
bio_14=raster("bio_14.asc")
bio_5=raster("bio_5.asc")
bio_6=raster("bio_6.asc")
BOSQUECULTIVADOASCMAXENT=raster("BOSQUECULTIVADOASCMAXENTB.asc")
ENCINOSINHERBASCMAXENTDIST=raster("ENCINOSINHERBASCMAXENTDIST.asc")
MESOFILOSINHERBASCMAXENTDIST=raster("MESOFILOSINHERBASCMAXENTDIST.asc")
OYAMELASCMAXENTDIST=raster("OYAMELASCMAXENTDIST.asc")
PASTIZALINDUCIDOASCMAXENT=raster("PASTIZALINDUCIDOASCMAXENTB.asc")
PASTIZALNATURALASCMAXENT=raster("PASTIZALNATURALASCMAXENTB.asc")
PASTIZALTODOASCMAXENT=raster("PASTIZALTODOASCMAXENTB.asc")
PINOASCMAXENTDIST=raster("PINOASCMAXENTDIST.asc")
VEGHIDROFILAASCMAXENT=raster("VEGHIDROFILAASCMAXENTB.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
SELVACADUCIFOLIAASCMAXENT=raster("SELVACADUCIFOLIAASCMAXENTB.asc")
SELVAALTAYBAJAPERENMAXENT=raster("SELVAALTAYBAJAPERENMAXENTB.asc")
ENCINOSINHERBASCMAXENTB=raster("ENCINOSINHERBASCMAXENTB.asc")
MESOFILOSINHERBASCMAXENTB=raster("MESOFILOSINHERBASCMAXENTB.asc")
OYAMELASCMAXENTB=raster("OYAMELASCMAXENTB.asc")
PINOASCMAXENTB=raster("PINOASCMAXENTB.asc")
pastizalaltamontañaASCS6=raster("pastizalaltamontañaASCS6.asc")


mex1=crop(Agriculturamaxent,mex)
mex2=crop(AGUAMAXENT,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(ARIDAASCMAXENT,mex)
mex5=crop(bio_13,mex)
mex6=crop(bio_14,mex)
mex7=crop(bio_5,mex)
mex8=crop(bio_6,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex10=crop(BOSQUECULTIVADOASCMAXENT,mex)
mex11=crop(ENCINOSINHERBASCMAXENTDIST,mex)
mex12=crop(MESOFILOSINHERBASCMAXENTDIST,mex)
mex13=crop(OYAMELASCMAXENTDIST,mex)
mex14=crop(PASTIZALINDUCIDOASCMAXENT,mex)
mex15=crop(PASTIZALNATURALASCMAXENT,mex)
mex16=crop(PASTIZALTODOASCMAXENT,mex)
mex17=crop(PINOASCMAXENTDIST,mex)
mex18=crop(VEGHIDROFILAASCMAXENT,mex)
mex19=crop(SLOPEBIENMAXENT,mex)
mex20=crop(SELVACADUCIFOLIAASCMAXENT,mex)
mex21=crop(SELVAALTAYBAJAPERENMAXENT,mex)
mex22=crop(ENCINOSINHERBASCMAXENTB,mex)
mex23=crop(MESOFILOSINHERBASCMAXENTB,mex)
mex24=crop(OYAMELASCMAXENTB,mex)
mex25=crop(PINOASCMAXENTB,mex)
mex26=crop(pastizalaltamontañaASCS6,mex)


mex1b=mask(mex1,mex)
mex2b=mask(mex2,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex10b=mask(mex10,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex18b=mask(mex18,mex)
mex19b=mask(mex19,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)
mex26b=mask(mex26,mex)



writeRaster(mex1b, "Agriculturaleprosa16.asc")
writeRaster(mex2b, "AGUAleprosa16.asc")
writeRaster(mex3b, "ALTITUDleprosa16.asc")
writeRaster(mex4b, "ARIDAleprosa16.asc")
writeRaster(mex5b, "bio_13leprosa16.asc")
writeRaster(mex6b, "bio_14leprosa16.asc")
writeRaster(mex7b, "bio_5leprosa16.asc")
writeRaster(mex8b, "bio_6leprosa16.asc")
writeRaster(mex9b, "ASPECTleprosa16.asc")
writeRaster(mex10b, "BOSQUECULTIVADOleprosa16.asc")
writeRaster(mex11b, "ENCINOSINHERBdistleprosa16.asc")
writeRaster(mex12b, "MESOFILOSINHERBdisleprosa16.asc")
writeRaster(mex13b, "OYAMELdistleprosa16.asc")
writeRaster(mex14b, "PASTIZALINDUCIDOleprosa16.asc")
writeRaster(mex15b, "PASTIZALNATURleprosa16.asc")
writeRaster(mex16b, "PASTIZALTODOleprosa16.asc")
writeRaster(mex17b, "PINOdistleprosa16.asc")
writeRaster(mex18b, "VEGHIDROFILAleprosa16.asc")
writeRaster(mex19b, "SLOPEleprosa16.asc")
writeRaster(mex20b, "SELVACADUCIFOLIAleprosa16.asc")
writeRaster(mex21b, "SELVAALTAYBAJAPERleprosa16.asc")
writeRaster(mex22b, "ENCINOSINHERBASleprosa16.asc")
writeRaster(mex23b, "MESOFILOSINHERBleprosa16.asc")
writeRaster(mex24b, "OYAMELleprosa16.asc")
writeRaster(mex25b, "PINOleprosa16.asc")
writeRaster(mex26b, "pastizalaltamontañaleprosa16.asc")




###ROBERTSI####

#########################para recortar las capas con shapes del area de estudio (M)############################

####se cargan los shps con los que se va a cortar las capas#####



mex=readOGR(".", "robertsieje")
plot(mex)


##########PARA RECORTAR LAS CAPAS CREADAS DE LA SERIE6###########################################################################

Agriculturamaxent=raster("AgriculturamaxentB.asc")
AGUAMAXENT=raster("aguamaxentB.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
ARIDAASCMAXENT=raster("ARIDAASCMAXENB.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio_13=raster("bio_13.asc")
bio_14=raster("bio_14.asc")
bio_5=raster("bio_5.asc")
bio_6=raster("bio_6.asc")
BOSQUECULTIVADOASCMAXENT=raster("BOSQUECULTIVADOASCMAXENTB.asc")
ENCINOSINHERBASCMAXENTDIST=raster("ENCINOSINHERBASCMAXENTDIST.asc")
MESOFILOSINHERBASCMAXENTDIST=raster("MESOFILOSINHERBASCMAXENTDIST.asc")
OYAMELASCMAXENTDIST=raster("OYAMELASCMAXENTDIST.asc")
PASTIZALINDUCIDOASCMAXENT=raster("PASTIZALINDUCIDOASCMAXENTB.asc")
PASTIZALNATURALASCMAXENT=raster("PASTIZALNATURALASCMAXENTB.asc")
PASTIZALTODOASCMAXENT=raster("PASTIZALTODOASCMAXENTB.asc")
PINOASCMAXENTDIST=raster("PINOASCMAXENTDIST.asc")
VEGHIDROFILAASCMAXENT=raster("VEGHIDROFILAASCMAXENTB.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
SELVACADUCIFOLIAASCMAXENT=raster("SELVACADUCIFOLIAASCMAXENTB.asc")
SELVAALTAYBAJAPERENMAXENT=raster("SELVAALTAYBAJAPERENMAXENTB.asc")
ENCINOSINHERBASCMAXENTB=raster("ENCINOSINHERBASCMAXENTB.asc")
MESOFILOSINHERBASCMAXENTB=raster("MESOFILOSINHERBASCMAXENTB.asc")
OYAMELASCMAXENTB=raster("OYAMELASCMAXENTB.asc")
PINOASCMAXENTB=raster("PINOASCMAXENTB.asc")
pastizalaltamontañaASCS6=raster("pastizalaltamontañaASCS6.asc")




mex1=crop(Agriculturamaxent,mex)
mex2=crop(AGUAMAXENT,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(ARIDAASCMAXENT,mex)
mex5=crop(bio_13,mex)
mex6=crop(bio_14,mex)
mex7=crop(bio_5,mex)
mex8=crop(bio_6,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex10=crop(BOSQUECULTIVADOASCMAXENT,mex)
mex11=crop(ENCINOSINHERBASCMAXENTDIST,mex)
mex12=crop(MESOFILOSINHERBASCMAXENTDIST,mex)
mex13=crop(OYAMELASCMAXENTDIST,mex)
mex14=crop(PASTIZALINDUCIDOASCMAXENT,mex)
mex15=crop(PASTIZALNATURALASCMAXENT,mex)
mex16=crop(PASTIZALTODOASCMAXENT,mex)
mex17=crop(PINOASCMAXENTDIST,mex)
mex18=crop(VEGHIDROFILAASCMAXENT,mex)
mex19=crop(SLOPEBIENMAXENT,mex)
mex20=crop(SELVACADUCIFOLIAASCMAXENT,mex)
mex21=crop(SELVAALTAYBAJAPERENMAXENT,mex)
mex22=crop(ENCINOSINHERBASCMAXENTB,mex)
mex23=crop(MESOFILOSINHERBASCMAXENTB,mex)
mex24=crop(OYAMELASCMAXENTB,mex)
mex25=crop(PINOASCMAXENTB,mex)
mex26=crop(pastizalaltamontañaASCS6,mex)


mex1b=mask(mex1,mex)
mex2b=mask(mex2,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex10b=mask(mex10,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex18b=mask(mex18,mex)
mex19b=mask(mex19,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)
mex26b=mask(mex26,mex)



writeRaster(mex1b, "Agriculturarobertsi16.asc")
writeRaster(mex2b, "AGUArobertsi16.asc")
writeRaster(mex3b, "ALTITUDrobertsi16.asc")
writeRaster(mex4b, "ARIDArobertsi16.asc")
writeRaster(mex5b, "bio_13robertsi16.asc")
writeRaster(mex6b, "bio_14robertsi16.asc")
writeRaster(mex7b, "bio_5robertsi16.asc")
writeRaster(mex8b, "bio_6robertsi16.asc")
writeRaster(mex9b, "ASPECTrobertsi16.asc")
writeRaster(mex10b, "BOSQUECULTIVADOrobertsi16.asc")
writeRaster(mex11b, "ENCINOSINHERBdistrobertsi16.asc")
writeRaster(mex12b, "MESOFILOSINHERBdisrobertsi16.asc")
writeRaster(mex13b, "OYAMELdistrobertsi16.asc")
writeRaster(mex14b, "PASTIZALINDUCIDOrobertsi16.asc")
writeRaster(mex15b, "PASTIZALNATURrobertsi16.asc")
writeRaster(mex16b, "PASTIZALTODOrobertsi16.asc")
writeRaster(mex17b, "PINOdistrobertsi16.asc")
writeRaster(mex18b, "VEGHIDROFILArobertsi16.asc")
writeRaster(mex19b, "SLOPErobertsi16.asc")
writeRaster(mex20b, "SELVACADUCIFOLIArobertsi16.asc")
writeRaster(mex21b, "SELVAALTAYBAJAPERrobertsi16.asc")
writeRaster(mex22b, "ENCINOSINHERBASrobertsi16.asc")
writeRaster(mex23b, "MESOFILOSINHERBrobertsi16.asc")
writeRaster(mex24b, "OYAMELrobertsi16.asc")
writeRaster(mex25b, "PINOrobertsi16.asc")
writeRaster(mex26b, "pastizalaltamontañarobertsi16.asc")






####se cargan los shps con los que se va a cortar las capas50#####



mex=readOGR(".", "belliiprovbien")
plot(mex)


agricultura2050=raster("agricultura2050.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
arida2050=raster("arida2050.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio13cc45bi50=raster("bio13cc45bi50.asc")
bio14cc45bi50=raster("bio14cc45bi50.asc")
bio5cc45bi50=raster("bio5cc45bi50.asc")
bio6cc45bi50=raster("bio6cc45bi50.asc")
encinodist2050=raster("encinodist2050.asc")
mesofilodist2050=raster("mesofilodist2050.asc")
oyameldist2050=raster("oyameldist2050.asc")
pastizalindcido2050=raster("pastizalindcido2050.asc")
pastizalnat2050=raster("pastizalnat2050.asc")
pastizaltodo2050=raster("pastizaltodo2050.asc")
pinodist2050=raster("pinodist2050.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
urbano2050=raster("urbano2050.asc")
encino2050=raster("encino2050.asc")
mesofilo2050=raster("mesofilo2050.asc")
oyamel2050=raster("oyamel2050.asc")
pino2050=raster("pino2050.asc")



mex1=crop(agricultura2050,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(arida2050,mex)
mex5=crop(bio13cc45bi50,mex)
mex6=crop(bio14cc45bi50,mex)
mex7=crop(bio5cc45bi50,mex)
mex8=crop(bio6cc45bi50,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex11=crop(encinodist2050,mex)
mex12=crop(mesofilodist2050,mex)
mex13=crop(oyameldist2050,mex)
mex14=crop(pastizalindcido2050,mex)
mex15=crop(pastizalnat2050,mex)
mex16=crop(pastizaltodo2050,mex)
mex17=crop(pinodist2050,mex)
mex20=crop(SLOPEBIENMAXENT,mex)
mex21=crop(urbano2050,mex)
mex22=crop(encino2050,mex)
mex23=crop(mesofilo2050,mex)
mex24=crop(oyamel2050,mex)
mex25=crop(pino2050,mex)



mex1b=mask(mex1,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)



writeRaster(mex1b, "agricultura2050bellii.asc")
writeRaster(mex3b, "ALTITUD2050bellii.asc")
writeRaster(mex4b, "arida2050bellii.asc")
writeRaster(mex5b, "bio13cc45bi50bellii.asc")
writeRaster(mex6b, "bio14cc45bi50bellii.asc")
writeRaster(mex7b, "bio5cc45bi50bellii.asc")
writeRaster(mex8b, "bio6cc45bi50bellii.asc")
writeRaster(mex9b, "ASPECT2050bellii.asc")
writeRaster(mex11b, "encinodist2050bellii.asc")
writeRaster(mex12b, "MESOFILOSINHERBdist2050bellii.asc")
writeRaster(mex13b, "mesofilodist2050bellii.asc")
writeRaster(mex14b, "pastizalindcido2050bellii.asc")
writeRaster(mex15b, "pastizalnat2050bellii.asc")
writeRaster(mex16b, "pastizaltodo2050bellii.asc")
writeRaster(mex17b, "pinodist2050bellii.asc")
writeRaster(mex20b, "SLOPE2050bellii.asc")
writeRaster(mex21b, "urbano2050bellii.asc")
writeRaster(mex22b, "encino2050bellii.asc")
writeRaster(mex23b, "mesofilo2050bellii.asc")
writeRaster(mex24b, "oyamel2050bellii.asc")
writeRaster(mex25b, "pino2050bellii.asc")





mex=readOGR(".", "cephalicaprov")
plot(mex)



agricultura2050=raster("agricultura2050.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
arida2050=raster("arida2050.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio13cc45bi50=raster("bio13cc45bi50.asc")
bio14cc45bi50=raster("bio14cc45bi50.asc")
bio5cc45bi50=raster("bio5cc45bi50.asc")
bio6cc45bi50=raster("bio6cc45bi50.asc")
encinodist2050=raster("encinodist2050.asc")
mesofilodist2050=raster("mesofilodist2050.asc")
oyameldist2050=raster("oyameldist2050.asc")
pastizalindcido2050=raster("pastizalindcido2050.asc")
pastizalnat2050=raster("pastizalnat2050.asc")
pastizaltodo2050=raster("pastizaltodo2050.asc")
pinodist2050=raster("pinodist2050.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
urbano2050=raster("urbano2050.asc")
encino2050=raster("encino2050.asc")
mesofilo2050=raster("mesofilo2050.asc")
oyamel2050=raster("oyamel2050.asc")
pino2050=raster("pino2050.asc")



mex1=crop(agricultura2050,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(arida2050,mex)
mex5=crop(bio13cc45bi50,mex)
mex6=crop(bio14cc45bi50,mex)
mex7=crop(bio5cc45bi50,mex)
mex8=crop(bio6cc45bi50,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex11=crop(encinodist2050,mex)
mex12=crop(mesofilodist2050,mex)
mex13=crop(oyameldist2050,mex)
mex14=crop(pastizalindcido2050,mex)
mex15=crop(pastizalnat2050,mex)
mex16=crop(pastizaltodo2050,mex)
mex17=crop(pinodist2050,mex)
mex20=crop(SLOPEBIENMAXENT,mex)
mex21=crop(urbano2050,mex)
mex22=crop(encino2050,mex)
mex23=crop(mesofilo2050,mex)
mex24=crop(oyamel2050,mex)
mex25=crop(pino2050,mex)



mex1b=mask(mex1,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)



writeRaster(mex1b, "agricultura2050cephalica.asc")
writeRaster(mex3b, "ALTITUD2050cephalica.asc")
writeRaster(mex4b, "arida2050cephalica.asc")
writeRaster(mex5b, "bio13cc45bi50cephalica.asc")
writeRaster(mex6b, "bio14cc45bi50cephalica.asc")
writeRaster(mex7b, "bio5cc45bi50cephalica.asc")
writeRaster(mex8b, "bio6cc45bi50cephalica.asc")
writeRaster(mex9b, "ASPECT2050cephalica.asc")
writeRaster(mex11b, "encinodist2050cephalica.asc")
writeRaster(mex12b, "MESOFILOSINHERBdist2050cephalica.asc")
writeRaster(mex13b, "mesofilodist2050cephalica.asc")
writeRaster(mex14b, "pastizalindcido2050cephalica.asc")
writeRaster(mex15b, "pastizalnat2050cephalica.asc")
writeRaster(mex16b, "pastizaltodo2050cephalica.asc")
writeRaster(mex17b, "pinodist2050cephalica.asc")
writeRaster(mex20b, "SLOPE2050cephalica.asc")
writeRaster(mex21b, "urbano2050cephalica.asc")
writeRaster(mex22b, "encino2050cephalica.asc")
writeRaster(mex23b, "mesofilo2050cephalica.asc")
writeRaster(mex24b, "oyamel2050cephalica.asc")
writeRaster(mex25b, "pino2050cephalica.asc")









mex=readOGR(".", "leprosaprov")
plot(mex)


agricultura2050=raster("agricultura2050.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
arida2050=raster("arida2050.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio13cc45bi50=raster("bio13cc45bi50.asc")
bio14cc45bi50=raster("bio14cc45bi50.asc")
bio5cc45bi50=raster("bio5cc45bi50.asc")
bio6cc45bi50=raster("bio6cc45bi50.asc")
encinodist2050=raster("encinodist2050.asc")
mesofilodist2050=raster("mesofilodist2050.asc")
oyameldist2050=raster("oyameldist2050.asc")
pastizalindcido2050=raster("pastizalindcido2050.asc")
pastizalnat2050=raster("pastizalnat2050.asc")
pastizaltodo2050=raster("pastizaltodo2050.asc")
pinodist2050=raster("pinodist2050.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
urbano2050=raster("urbano2050.asc")
encino2050=raster("encino2050.asc")
mesofilo2050=raster("mesofilo2050.asc")
oyamel2050=raster("oyamel2050.asc")
pino2050=raster("pino2050.asc")



mex1=crop(agricultura2050,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(arida2050,mex)
mex5=crop(bio13cc45bi50,mex)
mex6=crop(bio14cc45bi50,mex)
mex7=crop(bio5cc45bi50,mex)
mex8=crop(bio6cc45bi50,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex11=crop(encinodist2050,mex)
mex12=crop(mesofilodist2050,mex)
mex13=crop(oyameldist2050,mex)
mex14=crop(pastizalindcido2050,mex)
mex15=crop(pastizalnat2050,mex)
mex16=crop(pastizaltodo2050,mex)
mex17=crop(pinodist2050,mex)
mex20=crop(SLOPEBIENMAXENT,mex)
mex21=crop(urbano2050,mex)
mex22=crop(encino2050,mex)
mex23=crop(mesofilo2050,mex)
mex24=crop(oyamel2050,mex)
mex25=crop(pino2050,mex)



mex1b=mask(mex1,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)



writeRaster(mex1b, "agricultura2050leprosa.asc")
writeRaster(mex3b, "ALTITUD2050leprosa.asc")
writeRaster(mex4b, "arida2050leprosa.asc")
writeRaster(mex5b, "bio13cc45bi50leprosa.asc")
writeRaster(mex6b, "bio14cc45bi50leprosa.asc")
writeRaster(mex7b, "bio5cc45bi50leprosa.asc")
writeRaster(mex8b, "bio6cc45bi50leprosa.asc")
writeRaster(mex9b, "ASPECT2050leprosa.asc")
writeRaster(mex11b, "encinodist2050leprosa.asc")
writeRaster(mex12b, "MESOFILOSINHERBdist2050leprosa.asc")
writeRaster(mex13b, "mesofilodist2050leprosa.asc")
writeRaster(mex14b, "pastizalindcido2050leprosa.asc")
writeRaster(mex15b, "pastizalnat2050leprosa.asc")
writeRaster(mex16b, "pastizaltodo2050leprosa.asc")
writeRaster(mex17b, "pinodist2050leprosa.asc")
writeRaster(mex20b, "SLOPE2050leprosa.asc")
writeRaster(mex21b, "urbano2050leprosa.asc")
writeRaster(mex22b, "encino2050leprosa.asc")
writeRaster(mex23b, "mesofilo2050leprosa.asc")
writeRaster(mex24b, "oyamel2050leprosa.asc")
writeRaster(mex25b, "pino2050leprosa.asc")








mex=readOGR(".", "robertsieje")
plot(mex)



agricultura2050=raster("agricultura2050.asc")
ALTITUDBIENMAXENT=raster("ALTITUDBIENMAXENT.asc")
arida2050=raster("arida2050.asc")
ASPECTBIENMAXENT=raster("ASPECTBIENMAXENT.asc")
bio13cc45bi50=raster("bio13cc45bi50.asc")
bio14cc45bi50=raster("bio14cc45bi50.asc")
bio5cc45bi50=raster("bio5cc45bi50.asc")
bio6cc45bi50=raster("bio6cc45bi50.asc")
encinodist2050=raster("encinodist2050.asc")
mesofilodist2050=raster("mesofilodist2050.asc")
oyameldist2050=raster("oyameldist2050.asc")
pastizalindcido2050=raster("pastizalindcido2050.asc")
pastizalnat2050=raster("pastizalnat2050.asc")
pastizaltodo2050=raster("pastizaltodo2050.asc")
pinodist2050=raster("pinodist2050.asc")
SLOPEBIENMAXENT=raster("SLOPEBIENMAXENT.asc")
urbano2050=raster("urbano2050.asc")
encino2050=raster("encino2050.asc")
mesofilo2050=raster("mesofilo2050.asc")
oyamel2050=raster("oyamel2050.asc")
pino2050=raster("pino2050.asc")



mex1=crop(agricultura2050,mex)
mex3=crop(ALTITUDBIENMAXENT,mex)
mex4=crop(arida2050,mex)
mex5=crop(bio13cc45bi50,mex)
mex6=crop(bio14cc45bi50,mex)
mex7=crop(bio5cc45bi50,mex)
mex8=crop(bio6cc45bi50,mex)
mex9=crop(ASPECTBIENMAXENT,mex)
mex11=crop(encinodist2050,mex)
mex12=crop(mesofilodist2050,mex)
mex13=crop(oyameldist2050,mex)
mex14=crop(pastizalindcido2050,mex)
mex15=crop(pastizalnat2050,mex)
mex16=crop(pastizaltodo2050,mex)
mex17=crop(pinodist2050,mex)
mex20=crop(SLOPEBIENMAXENT,mex)
mex21=crop(urbano2050,mex)
mex22=crop(encino2050,mex)
mex23=crop(mesofilo2050,mex)
mex24=crop(oyamel2050,mex)
mex25=crop(pino2050,mex)



mex1b=mask(mex1,mex)
mex3b=mask(mex3,mex)
mex4b=mask(mex4,mex)
mex5b=mask(mex5,mex)
mex6b=mask(mex6,mex)
mex7b=mask(mex7,mex)
mex8b=mask(mex8,mex)
mex9b=mask(mex9,mex)
mex11b=mask(mex11,mex)
mex12b=mask(mex12,mex)
mex13b=mask(mex13,mex)
mex14b=mask(mex14,mex)
mex15b=mask(mex15,mex)
mex16b=mask(mex16,mex)
mex17b=mask(mex17,mex)
mex20b=mask(mex20,mex)
mex21b=mask(mex21,mex)
mex22b=mask(mex22,mex)
mex23b=mask(mex23,mex)
mex24b=mask(mex24,mex)
mex25b=mask(mex25,mex)



writeRaster(mex1b, "agricultura2050robertsi.asc")
writeRaster(mex3b, "ALTITUD2050robertsi.asc")
writeRaster(mex4b, "arida2050robertsi.asc")
writeRaster(mex5b, "bio13cc45bi50robertsi.asc")
writeRaster(mex6b, "bio14cc45bi50robertsi.asc")
writeRaster(mex7b, "bio5cc45bi50robertsi.asc")
writeRaster(mex8b, "bio6cc45bi50robertsi.asc")
writeRaster(mex9b, "ASPECT2050robertsi.asc")
writeRaster(mex11b, "encinodist2050robertsi.asc")
writeRaster(mex12b, "MESOFILOSINHERBdist2050robertsi.asc")
writeRaster(mex13b, "mesofilodist2050robertsi.asc")
writeRaster(mex14b, "pastizalindcido2050robertsi.asc")
writeRaster(mex15b, "pastizalnat2050robertsi.asc")
writeRaster(mex16b, "pastizaltodo2050robertsi.asc")
writeRaster(mex17b, "pinodist2050robertsi.asc")
writeRaster(mex20b, "SLOPE2050robertsi.asc")
writeRaster(mex21b, "urbano2050robertsi.asc")
writeRaster(mex22b, "encino2050robertsi.asc")
writeRaster(mex23b, "mesofilo2050robertsi.asc")
writeRaster(mex24b, "oyamel2050robertsi.asc")
writeRaster(mex25b, "pino2050robertsi.asc")


####cortar las capas de urban para cada especie 2016#####

mex=readOGR(".", "belliiprovbien")
plot(mex)


urbanbelli16=raster("urban016.asc")
mex1=crop(urbanbelli16,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanbelli16.asc")





mex=readOGR(".", "cephalicaprov")
plot(mex)

urbancephalica16=raster("urban016.asc")
mex1=crop(urbanbelli16,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbancephalica16.asc")




mex=readOGR(".", "leprosaprov")
plot(mex)


urbanleprosa16=raster("urban016.asc")
mex1=crop(urbanleprosa16,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanleprosa16.asc")



mex=readOGR(".", "robertsieje")
plot(mex)

urbanrobert16=raster("urban016.asc")
mex1=crop(urbanrobert16,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanrobert16.asc")



####cortar las capas de urban para cada especie 2050#####


mex=readOGR(".", "belliiprovbien")
plot(mex)


urbanbelli50=raster("urban2050.asc")
mex1=crop(urbanbelli50,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanbelli50.asc")


mex=readOGR(".", "cephalicaprov")
plot(mex)

urbancephalica50=raster("urban2050.asc")
mex1=crop(urbanbelli50,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbancephalica50.asc")




mex=readOGR(".", "leprosaprov")
plot(mex)


urbanleprosa50=raster("urban2050.asc")
mex1=crop(urbanleprosa50,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanleprosa50.asc")



mex=readOGR(".", "robertsieje")
plot(mex)

urbanrobert50=raster("urban2050.asc")
mex1=crop(urbanrobert50,mex)
mex1b=mask(mex1,mex)
writeRaster(mex1b, "urbanrobert50.asc")


############para eliminar las zonas de urbanizacion la capa de modelado de MAXENT 2016###################

hacemos una capa donde la urbanizacion es = 0
y todo el resto es =-9999 esto lo hice en idrisi con RECLASS

luego para unir las capas en R

urbanbellii=raster("urbanbelli16.asc") ##cargamos la capa de urbanizacion###
albbel=raster("Isthmura_bellii_avg.asc") ##cargamos la capa del modelado###
alburbanbellii=merge(urbanbellii,albbel) ###con este comando se unen###
plot(alburbanbellii)
writeRaster(alburbanbellii, "Isthmura_bellii_avg2016sinurban.asc")


urbanceph=raster("urbancephalica16.asc") ##cargamos la capa de urbanizacion###
albceph=raster("Aquiloeurycea_cephalica_avg.asc") ##cargamos la capa del modelado###
alburbanceph=merge(urbanceph,albceph) ###con este comando se unen###
plot(alburbanceph)
writeRaster(alburbanceph, "Aquiloeurycea_cephalica_avg2016sinurban.asc")


urbanlep=raster("urbanleprosa16.asc") ##cargamos la capa de urbanizacion###
alblep=raster("Pseudoeurycea_leprosa_avg.asc") ##cargamos la capa del modelado###
alburbanlep=merge(urbanbellii,alblep) ###con este comando se unen###
plot(alburbanlep)
writeRaster(alburbanlep, "Pseudoeurycea_leprosa_avg2016sinurban.asc")

urbanrob=raster("urbanrobert16.asc") ##cargamos la capa de urbanizacion###
albrob=raster("Pseudoeurycea_robertsi_avg.asc") ##cargamos la capa del modelado###
alburbanrob=merge(urbanrob,albrob) ###con este comando se unen###
plot(alburbanrob)
writeRaster(alburbanrob, "Pseudoeurycea_robertsi_avg2016sinurban.asc")




############para eliminar las zonas de urbanizacion la capa de modelado de MAXENT 2050###################

hacemos una capa donde la urbanizacion es = 0
y todo el resto es =-9999 esto lo hice en idrisi con RECLASS

luego para unir las capas en R

urbanbellii=raster("urbanbelli50.asc") ##cargamos la capa de urbanizacion###
albbel=raster("Isthmura_bellii_avg.asc") ##cargamos la capa del modelado###
alburbanbellii=merge(urbanbellii,albbel) ###con este comando se unen###
plot(alburbanbellii)
writeRaster(alburbanbellii, "Isthmura_bellii_avg2050sinurban.asc")


urbanceph=raster("urbancephalica50.asc") ##cargamos la capa de urbanizacion###
albceph=raster("Aquiloeurycea_cephalica_avg.asc") ##cargamos la capa del modelado###
alburbanceph=merge(urbanceph,albceph) ###con este comando se unen###
plot(alburbanceph)
writeRaster(alburbanceph, "Aquiloeurycea_cephalica_avg2050sinurban.asc")


urbanlep=raster("urbanleprosa50.asc") ##cargamos la capa de urbanizacion###
alblep=raster("Pseudoeurycea_leprosa_avg.asc") ##cargamos la capa del modelado###
alburbanlep=merge(urbanbellii,alblep) ###con este comando se unen###
plot(alburbanlep)
writeRaster(alburbanlep, "Pseudoeurycea_leprosa_avg2050sinurban.asc")

urbanrob=raster("urbanrobert50.asc") ##cargamos la capa de urbanizacion###
albrob=raster("Pseudoeurycea_robertsi_avg.asc") ##cargamos la capa del modelado###
alburbanrob=merge(urbanrob,albrob) ###con este comando se unen###
plot(alburbanrob)
writeRaster(alburbanrob, "Pseudoeurycea_robertsi_avg2050sinurban.asc")



#################graficar todos los mapas generados######################


E116=raster("Isthmura_bellii_avg2016sinurban.asc")
E216=raster("Aquiloeurycea_cephalica_avg2016sinurban.asc")
E316=raster("Pseudoeurycea_leprosa_avg2016sinurban.asc")
E416=raster("Pseudoeurycea_robertsi_avg2016sinurban.asc")

F1=raster("Isthmura_bellii_avg2050sinurban.asc")
F2=raster("Aquiloeurycea_cephalica_avg2050sinurban.asc")
F3=raster("Pseudoeurycea_leprosa_avg2050sinurban.asc")
F4=raster("Pseudoeurycea_robertsi_avg2050sinurban.asc")


#####para guardar los mapas en pdf########

pdf("Isthmura_bellii_avg2016sinurban.pdf", height=10, width=10)
plot(E116)
dev.off()

pdf("Aquiloeurycea_cephalica_avg2016sinurban.pdf", height=10, width=10)
plot(E216)
dev.off()

pdf("Pseudoeurycea_leprosa_avg2016sinurban.pdf", height=10, width=10)
plot(E316)
dev.off()

pdf("Pseudoeurycea_robertsi_avg2016sinurban.pdf", height=10, width=10)
plot(E416)
dev.off()




pdf("Isthmura_bellii_avg2050sinurban.pdf", height=10, width=10)
plot(F1)
dev.off()

pdf("Aquiloeurycea_cephalica_avg2050sinurban.pdf", height=10, width=10)
plot(F2)
dev.off()

pdf("Pseudoeurycea_leprosa_avg2050sinurban.pdf", height=10, width=10)
plot(F3)
dev.off()

pdf("Pseudoeurycea_robertsi_avg2050sinurban.pdf", height=10, width=10)
plot(F4)
dev.off()




#####################################PARA CALCULAR LAS AREAS DE SUITABILITY EN KM2 PRESENTE################################



bellii=raster("Isthmura_bellii_avg2016sinurban.asc")
m.df <- as.data.frame(bellii, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Isthmura_bellii_avg2016sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_bellii<-length(cell_size1)*median(cell_size1)
raster_area_bellii



cephalica=raster("Aquiloeurycea_cephalica_avg2016sinurban.asc")
m.df <- as.data.frame(cephalica, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Aquiloeurycea_cephalica_avg2016sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_cephalica<-length(cell_size1)*median(cell_size1)
raster_area_cephalica

leprosa=raster("Pseudoeurycea_leprosa_avg2016sinurban.asc")
m.df <- as.data.frame(leprosa, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_leprosa_avg2016sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_leprosa<-length(cell_size1)*median(cell_size1)
raster_area_leprosa

robertsi=raster("Pseudoeurycea_robertsi_avg2016sinurban.asc")
m.df <- as.data.frame(robertsi, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_robertsi_avg2016sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_robertsi<-length(cell_size1)*median(cell_size1)
raster_area_robertsi




#####################################PARA CALCULAR LAS AREAS DE SUITABILITY EN KM2 FUTURO################################



bellii=raster("Isthmura_bellii_avg2050sinurban.asc")
m.df <- as.data.frame(bellii, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Isthmura_bellii_avg2050sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_bellii<-length(cell_size1)*median(cell_size1)
raster_area_bellii



cephalica=raster("Aquiloeurycea_cephalica_avg2050sinurban.asc")
m.df <- as.data.frame(cephalica, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Aquiloeurycea_cephalica_avg2050sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_cephalica<-length(cell_size1)*median(cell_size1)
raster_area_cephalica

leprosa=raster("Pseudoeurycea_leprosa_avg2050sinurban.asc")
m.df <- as.data.frame(leprosa, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_leprosa_avg2050sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_leprosa<-length(cell_size1)*median(cell_size1)
raster_area_leprosa

robertsi=raster("Pseudoeurycea_robertsi_avg2050sinurban.asc")
m.df <- as.data.frame(robertsi, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_robertsi_avg2050sinurban> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_robertsi<-length(cell_size1)*median(cell_size1)
raster_area_robertsi


VALORES PRESNETE  0.6

bellii =52508.06
cephalica=15465.64
leprosa= 4398.106
robertsi=310.9741


VALORES FUTURO  0.6


bellii =54110.56
cephalica=15289.12
leprosa= 4975.155
robertsi=305.3047




VALORES PRESNETE  0.8

bellii =2639.892
cephalica=2646.933
leprosa= 799.1241
robertsi=8.88943    8.88943


VALORES FUTURO  0.8


bellii =1996.616
cephalica=2717.417
leprosa=  823.4232
robertsi=29.88883






robertsi=raster("Pseudoeurycea_robertsi_avg.asc")
m.df <- as.data.frame(robertsi, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_robertsi_avg> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_robertsi<-length(cell_size1)*median(cell_size1)
raster_area_robertsi








robertsi=raster("Pseudoeurycea_robertsi_avg.asc")
m.df <- as.data.frame(robertsi, xy=TRUE)
 m.df1 <- na.omit(m.df)
m.df2 <- m.df1[m.df1$Pseudoeurycea_robertsi_avg> 0.8,] ###EL 0.8 ES EL AREA DE SUITABILITY A PARTIR DE QUE QUEREMOS CALCULAR EL AREA######keep only cells that that have a suitability score above 0.5 (scores range from 0 to 1)
m.raster <- rasterFromXYZ(m.df2)
cell_size<-area(m.raster, na.rm=TRUE, weights=FALSE)
cell_size1<-cell_size[!is.na(cell_size)]
raster_area_robertsi<-length(cell_size1)*median(cell_size1)
raster_area_robertsi



##########ENMEVAL###########################################################################


###bellii#####

agri=raster("agricultura2050bellii.asc")
ALT=raster("ALTITUD2050bellii.asc")
arid=raster("arida2050bellii.asc")
ASPECT=raster("ASPECT2050bellii.asc")
bio13=raster("bio13cc45bi50bellii.asc")
bio14=raster("bio14cc45bi50bellii.asc")
bio5=raster("bio5cc45bi50bellii.asc")
bio6=raster("bio6cc45bi50bellii.asc")
past=raster("pastizaltodo2050bellii.asc")
SLOPE=raster("SLOPE2050bellii.asc")
encino=raster("encino2050bellii.asc")
mesofilo=raster("MESOFILOSINHERBdist2050bellii.asc")
oyamel=raster("oyamel2050bellii.asc")
pino=raster("pino2050bellii.asc")

bv=read.csv("ibelliENMEVAL.csv")


#Convert to data frame#
#Convertir a data frame#

occs=as.data.frame(bv[,1:2])
plot(occs)

envs=stack(agri, ALT, arid, ASPECT, bio13, bio14, bio5, bio6, past, SLOPE, encino, mesofilo, oyamel, pino)

#to plot all layers #
#para graficar todas las capas#
plot(envs)

#to plot the first layer #
#para graficar la primera capa#

plot(envs[[1]],main=names(envs)[1])

#to see the points on the layers #
#para ver los puntos sobre las capas#

points(occs)

library(sp)

#convert data frame of points becomes an object #
#Para que el data frame de puntos se vuelva un objeto#

occs.sp=SpatialPoints(occs)


library(ENMeval)

#Generation of 10000 points of all environmental variables#
#Generacion de 10000 puntos de todas las variables ambientales#

bg=randomPoints(envs,n=10000)
plot(bg)

#to convert to data frame#
#para convertir a data frame#

bg=as.data.frame(bg)

#so that the points that were generated are distributed in the study area in a homogeneous way #
#para que los puntos que se generaron se distribuyen en la zona de estudio de manera homogenia#

plot(envs[[1]],legend=FALSE)
points(bg, col='red')

##models we test##
##modelos puestos a prueba##

checkerboard1analisisb=ENMevaluate(occs, envs, bg, method='checkerboard1', RMvalues=seq(1,2), fc=c("L", "LQ", "H", "LQH", "LQHP", "LQHPT"),aggregation.factor = c(2, 2), algorithm='maxent.jar',parallel=TRUE)

AIC=checkerboard1analisisb@results[which(checkerboard1analisisb@results$delta.AICc==0),]
write.csv(AIC,"belliiAICchkb2.csv")



###cepalica#############


agri=raster("agricultura2050cephalica.asc")
ALT=raster("ALTITUD2050cephalica.asc")
arid=raster("arida2050cephalica.asc")
ASPECT=raster("ASPECT2050cephalica.asc")
bio13=raster("bio13cc45bi50cephalica.asc")
bio14=raster("bio14cc45bi50cephalica.asc")
bio5=raster("bio5cc45bi50cephalica.asc")
bio6=raster("bio6cc45bi50cephalica.asc")
past=raster("pastizaltodo2050cephalica.asc")
SLOPE=raster("SLOPE2050cephalica.asc")
encino=raster("encino2050cephalica.asc")
mesofilo=raster("MESOFILOSINHERBdist2050cephalica.asc")
oyamel=raster("oyamel2050cephalica.asc")
pino=raster("pino2050cephalica.asc")

bv=read.csv("cepENMEVAL.csv")



#Convert to data frame#
#Convertir a data frame#

occs=as.data.frame(bv[,1:2])
plot(occs)

envs=stack(agri, ALT, arid, ASPECT, bio13, bio14, bio5, bio6, past, SLOPE, encino, mesofilo, oyamel, pino)

#to plot all layers #
#para graficar todas las capas#
plot(envs)

#to plot the first layer #
#para graficar la primera capa#

plot(envs[[1]],main=names(envs)[1])

#to see the points on the layers #
#para ver los puntos sobre las capas#

points(occs)

library(sp)

#convert data frame of points becomes an object #
#Para que el data frame de puntos se vuelva un objeto#

occs.sp=SpatialPoints(occs)


library(ENMeval)

#Generation of 10000 points of all environmental variables#
#Generacion de 10000 puntos de todas las variables ambientales#

bg=randomPoints(envs,n=10000)
plot(bg)

#to convert to data frame#
#para convertir a data frame#

bg=as.data.frame(bg)

#so that the points that were generated are distributed in the study area in a homogeneous way #
#para que los puntos que se generaron se distribuyen en la zona de estudio de manera homogenia#

plot(envs[[1]],legend=FALSE)
points(bg, col='red')

##models we test##
##modelos puestos a prueba##

checkerboard1analisisb=ENMevaluate(occs, envs, bg, method='checkerboard1', RMvalues=seq(1,2), fc=c("L", "LQ", "H", "LQH", "LQHP", "LQHPT"),aggregation.factor = c(2, 2), algorithm='maxent.jar',parallel=TRUE)

AIC=checkerboard1analisisb@results[which(checkerboard1analisisb@results$delta.AICc==0),]
write.csv(AIC,"cepAICchkb2.csv")

#####leprosa######



agri=raster("agricultura2050leprosa.asc")
ALT=raster("ALTITUD2050leprosa.asc")
arid=raster("arida2050leprosa.asc")
ASPECT=raster("ASPECT2050leprosa.asc")
bio13=raster("bio13cc45bi50leprosa.asc")
bio14=raster("bio14cc45bi50leprosa.asc")
bio5=raster("bio5cc45bi50leprosa.asc")
bio6=raster("bio6cc45bi50leprosa.asc")
past=raster("pastizaltodo2050leprosa.asc")
SLOPE=raster("SLOPE2050leprosa.asc")
encino=raster("encino2050leprosa.asc")
mesofilo=raster("MESOFILOSINHERBdist2050leprosa.asc")
oyamel=raster("oyamel2050leprosa.asc")
pino=raster("pino2050leprosa.asc")

bv=read.csv("lepENMEVAL.csv")



#Convert to data frame#
#Convertir a data frame#

occs=as.data.frame(bv[,1:2])
plot(occs)

envs=stack(agri, ALT, arid, ASPECT, bio13, bio14, bio5, bio6, past, SLOPE, encino, mesofilo, oyamel, pino)

#to plot all layers #
#para graficar todas las capas#
plot(envs)

#to plot the first layer #
#para graficar la primera capa#

plot(envs[[1]],main=names(envs)[1])

#to see the points on the layers #
#para ver los puntos sobre las capas#

points(occs)

library(sp)

#convert data frame of points becomes an object #
#Para que el data frame de puntos se vuelva un objeto#

occs.sp=SpatialPoints(occs)


library(ENMeval)

#Generation of 10000 points of all environmental variables#
#Generacion de 10000 puntos de todas las variables ambientales#

bg=randomPoints(envs,n=10000)
plot(bg)

#to convert to data frame#
#para convertir a data frame#

bg=as.data.frame(bg)

#so that the points that were generated are distributed in the study area in a homogeneous way #
#para que los puntos que se generaron se distribuyen en la zona de estudio de manera homogenia#

plot(envs[[1]],legend=FALSE)
points(bg, col='red')

##models we test##
##modelos puestos a prueba##

checkerboard1analisisb=ENMevaluate(occs, envs, bg, method='checkerboard1', RMvalues=seq(1,2), fc=c("L", "LQ", "H", "LQH", "LQHP", "LQHPT"),aggregation.factor = c(2, 2), algorithm='maxent.jar',parallel=TRUE)

AIC=checkerboard1analisisb@results[which(checkerboard1analisisb@results$delta.AICc==0),]
write.csv(AIC,"leprosaAICchkb2.csv")

#######robertsi######################




agri=raster("agricultura2050robertsi.asc")
ALT=raster("ALTITUD2050robertsi.asc")
arid=raster("arida2050robertsi.asc")
ASPECT=raster("ASPECT2050robertsi.asc")
bio13=raster("bio13cc45bi50robertsi.asc")
bio14=raster("bio14cc45bi50robertsi.asc")
bio5=raster("bio5cc45bi50robertsi.asc")
bio6=raster("bio6cc45bi50robertsi.asc")
past=raster("pastizaltodo2050robertsi.asc")
SLOPE=raster("SLOPE2050robertsi.asc")
encino=raster("encino2050robertsi.asc")
mesofilo=raster("MESOFILOSINHERBdist2050robertsi.asc")
oyamel=raster("oyamel2050robertsi.asc")
pino=raster("pino2050robertsi.asc")

bv=read.csv("robENMEVAL.csv")



#Convert to data frame#
#Convertir a data frame#

occs=as.data.frame(bv[,1:2])
plot(occs)

envs=stack(agri, ALT, arid, ASPECT, bio13, bio14, bio5, bio6, past, SLOPE, encino, mesofilo, oyamel, pino)

#to plot all layers #
#para graficar todas las capas#
plot(envs)

#to plot the first layer #
#para graficar la primera capa#

plot(envs[[1]],main=names(envs)[1])

#to see the points on the layers #
#para ver los puntos sobre las capas#

points(occs)

library(sp)

#convert data frame of points becomes an object #
#Para que el data frame de puntos se vuelva un objeto#

occs.sp=SpatialPoints(occs)


library(ENMeval)

#Generation of 10000 points of all environmental variables#
#Generacion de 10000 puntos de todas las variables ambientales#

bg=randomPoints(envs,n=10000)
plot(bg)

#to convert to data frame#
#para convertir a data frame#

bg=as.data.frame(bg)

#so that the points that were generated are distributed in the study area in a homogeneous way #
#para que los puntos que se generaron se distribuyen en la zona de estudio de manera homogenia#

plot(envs[[1]],legend=FALSE)
points(bg, col='red')

##models we test##
##modelos puestos a prueba##

checkerboard1analisisb=ENMevaluate(occs, envs, bg, method='checkerboard1', RMvalues=seq(1,2), fc=c("L", "LQ", "H", "LQH", "LQHP", "LQHPT"),aggregation.factor = c(2, 2), algorithm='maxent.jar',parallel=TRUE)

AIC=checkerboard1analisisb@results[which(checkerboard1analisisb@results$delta.AICc==0),]
write.csv(AIC,"robertsiAICchkb2.csv")