TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#==================================================
# build a support library

LIBRARY_IOC += sqlite

# xxxRecord.h will be created from xxxRecord.dbd
#DBDINC += xxxRecord
# install sqlite.dbd into <top>/dbd
DBD += sqlite.dbd

INC += sqlite3.h

# specify all source files to be compiled and added to the library
sqlite_SRCS += sqlite3.c

sqlite_LIBS += $(EPICS_BASE_IOC_LIBS)

#USR_LDFLAGS_WIN32 += /DEF:../sqlite3.def

#ifeq ($(SHARED_LIBRARIES),YES)
#USR_CFLAGS_WIN32 += -DSQLITE_API=__declspec(dllexport)
#endif

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

