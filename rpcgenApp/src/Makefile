TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#==================================================
# build a support library

PROD_IOC += portmap rpcgen

SRC_DIRS += $(ONCRPC)/win32/librpc $(ONCRPC)/win32/rpcgen

USR_CPPFLAGS += -DWIN32 -D_NT -D_WINDOWS -I$(ONCRPC)/win32/include

portmap_SRCS += portmap.c
portmap_LIBS += oncrpc
portmap_SYS_LIBS_WIN32 += ws2_32

rpcgen_SRCS += rpc_main.c rpc_hout.c rpc_cout.c rpc_pars.c rpc_scan.c rpc_util.c rpc_svco.c rpc_clnt.c
rpcgen_LIBS += oncrpc
rpcgen_SYS_LIBS_WIN32 += ws2_32

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

