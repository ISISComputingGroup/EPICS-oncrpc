TOP=../..

include $(TOP)/configure/CONFIG
#----------------------------------------
#  ADD MACRO DEFINITIONS AFTER THIS LINE
#=============================

#==================================================
# build a support library

LIBRARY_IOC += oncrpc

# specify all source files to be compiled and added to the library
SRC_DIRS += $(ONCRPC)/win32/include $(ONCRPC)/win32/librpc

oncrpc_SRCS += \
		CLNT_RAW.c \
		XDR.c \
		CLNT_TCP.c \
		CLNT_UDP.c \
		PMAP_RMT.c \
		RPC_PROT.c \
		SVC_AUTU.c \
		SVC_AUTH.c \
		SVC_RAW.c \
		SVC_RUN.c \
		SVC_TCP.c \
		SVC_UDP.c \
		XDR_MEM.c \
		XDR_REC.c \
		AUTH_NON.c \
		AUTH_UNI.c \
		AUTHUNIX.c \
		BINDRESV.c \
		CLNT_GEN.c \
		CLNT_PER.c \
		CLNT_SIM.c \
		GET_MYAD.c \
		GETRPCEN.c \
		GETRPCPO.c \
		PMAP_CLN.c \
		PMAP_GET.c \
		PMAP_GMA.c \
		PMAP_PRO.c \
		PMAP_PR.c \
		RPC_CALL.c \
		RPC_COMM.c \
		SVC_SIMP.c \
		XDR_ARRA.c \
		XDR_FLOA.c \
		XDR_REFE.c \
		XDR_STDI.c \
		SVC.c \
		BCOPY.c \
		NT.c

INC += rpc/auth.h rpc/auth_uni.h rpc/bcopy.h rpc/clnt.h rpc/Netdb.h rpc/Pmap_cln.h \
		rpc/Pmap_pro.h rpc/pmap_rmt.h rpc/Rpc.h rpc/rpc_msg.h rpc/svc.h rpc/svc_auth.h \
		rpc/types.h rpc/xdr.h

USR_CPPFLAGS += -DWIN32 -D_NT -D_WINDOWS -DONCRPCDLL

oncrpc_SYS_LIBS_WIN32 += ws2_32 advapi32

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE

