#############################################################################
# Makefile for building ta_common_cmd
# Generated by tmake;
#     Project: ta_common/ta_common
#    Template: lib
#############################################################################

####### Compiler, tools and options

CC	=	sc
CXX	=	sc
CFLAGS	=	-mn -w2 -g -DTA_DEBUG -D_DEBUG -DWIN32
CXXFLAGS=	-mn -w2 -g -DTA_DEBUG -D_DEBUG -DWIN32
INCPATH	=	-I"..\..\..\..\..\src\ta_common" -I"..\..\..\..\..\include"
LIB	=	lib /C /N /NOI /P:32
MOC	=	moc

ZIP	=	zip -r -9

####### Files

HEADERS =	
SOURCES =	..\..\..\..\..\src\ta_common\ta_global.c \
		..\..\..\..\..\src\ta_common\ta_retcode.c \
		..\..\..\..\..\src\ta_common\ta_version.c
OBJECTS =	..\..\..\..\..\temp\cmd\ta_global.obj \
		..\..\..\..\..\temp\cmd\ta_retcode.obj \
		..\..\..\..\..\temp\cmd\ta_version.obj
SRCMOC	=	
OBJMOC	=	
DIST	=	
TARGET	=	..\..\..\..\..\lib\ta_common_cmd.lib

####### Implicit rules

.SUFFIXES: .cpp .cxx .cc .c

.cpp.obj:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o$@ $<

.cxx.obj:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o$@ $<

.cc.obj:
	$(CXX) -c $(CXXFLAGS) $(INCPATH) -o$@ $<

.c.obj:
	$(CC) -c $(CFLAGS) $(INCPATH) -o$@ $<

####### Build rules

all: $(TARGET)

$(TARGET): $(OBJECTS) $(OBJMOC) 
	-del $(TARGET)
	$(LIB) $(TARGET) ..\..\..\..\..\temp\cmd\ta_global.obj \
+..\..\..\..\..\temp\cmd\ta_retcode.obj \
+..\..\..\..\..\temp\cmd\ta_version.obj \
+,;

moc: $(SRCMOC)

tmake: ../cmd/win32/symantec/ta_common/Makefile

../cmd/win32/symantec/ta_common/Makefile: ta_common/ta_common.pro
	tmake ta_common/ta_common.pro -o ../cmd/win32/symantec/ta_common/Makefile

dist:
	$(ZIP) ta_common/ta_common.zip ta_common/ta_common.pro $(SOURCES) $(HEADERS) $(DIST)

clean:
	-del ..\..\..\..\..\temp\cmd\ta_global.obj
	-del ..\..\..\..\..\temp\cmd\ta_retcode.obj
	-del ..\..\..\..\..\temp\cmd\ta_version.obj
	-del $(TARGET)
	-del ../../../../../bin/*.map
	-del ../../../../../bin/*._xe
	-del ../../../../../bin/*.tds
	-del ../../../../../bin/*.pdb
	-del ../../../../../bin/*.pbo
	-del ../../../../../bin/*.pbi
	-del ../../../../../bin/*.pbt
	-del ../../../../../temp/cmd/*.pch
	-del ../../../../../temp/cmd/*.idb
	-del ../../../../../temp/cmd/ta_common_cmd/*.pch
	-del ../../../../../temp/cmd/ta_common_cmd/*.idb
	-del ../../../../../temp/cmd/ta_common_cmd/*.obj

####### Compile

..\..\..\..\..\temp\cmd\ta_global.obj: ..\..\..\..\..\src\ta_common\ta_global.c
	$(CC) -c $(CFLAGS) $(INCPATH) -o..\..\..\..\..\temp\cmd\ta_global.obj ..\..\..\..\..\src\ta_common\ta_global.c

..\..\..\..\..\temp\cmd\ta_retcode.obj: ..\..\..\..\..\src\ta_common\ta_retcode.c
	$(CC) -c $(CFLAGS) $(INCPATH) -o..\..\..\..\..\temp\cmd\ta_retcode.obj ..\..\..\..\..\src\ta_common\ta_retcode.c

..\..\..\..\..\temp\cmd\ta_version.obj: ..\..\..\..\..\src\ta_common\ta_version.c
	$(CC) -c $(CFLAGS) $(INCPATH) -o..\..\..\..\..\temp\cmd\ta_version.obj ..\..\..\..\..\src\ta_common\ta_version.c

