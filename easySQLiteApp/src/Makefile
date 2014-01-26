TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#==================================================
# build a support library

LIBRARY_IOC += easySQLite

# xxxRecord.h will be created from xxxRecord.dbd
#DBDINC += xxxRecord
# install easySQLite.dbd into <top>/dbd
DBD += easySQLite.dbd

INC += SqlCommon.h SqlDatabase.h SqlTable.h SqlField.h SqlTable.h SqlFieldSet.h SqlRecordSet.h SqlRecord.h SqlValue.h

# specify all source files to be compiled and added to the library
easySQLite_SRCS += SHA1.cpp SqlCommon.cpp SqlDatabase.cpp SqlField.cpp SqlFieldSet.cpp SqlRecord.cpp SqlRecordSet.cpp SqlTable.cpp SqlValue.cpp

easySQLite_LIBS += sqlite $(EPICS_BASE_IOC_LIBS)

ifeq ($(SHARED_LIBRARIES),YES)
USR_CPPFLAGS_WIN32 += -DEASYSQLITE_EXPORT
endif
#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

