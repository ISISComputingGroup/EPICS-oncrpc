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
		clnt_raw.c \
		Xdr.c \
		Clnt_tcp.c \
		Clnt_udp.c \
		Pmap_rmt.c \
		rpc_prot.c \
		Svc_autu.c \
		svc_auth.c \
		svc_raw.c \
		Svc_run.c \
		Svc_tcp.c \
		Svc_udp.c \
		xdr_mem.c \
		Xdr_rec.c \
		Auth_non.c \
		Auth_uni.c \
		authunix.c \
		Bindresv.c \
		clnt_gen.c \
		Clnt_per.c \
		clnt_sim.c \
		Get_myad.c \
		Getrpcen.c \
		Getrpcpo.c \
		Pmap_cln.c \
		pmap_get.c \
		pmap_gma.c \
		pmap_pro.c \
		pmap_pr.c \
		rpc_call.c \
		rpc_comm.c \
		Svc_simp.c \
		Xdr_arra.c \
		xdr_floa.c \
		Xdr_refe.c \
		xdr_stdi.c \
		Svc.c \
		bcopy.c \
		nt.c
		
USR_CPPFLAGS += -DWIN32 -D_NT -D_WINDOWS -DONCRPCDLL

oncrpc_SYS_LIBS_WIN32 += ws2_32 advapi32

#===========================

include $(TOP)/configure/RULES
#----------------------------------------
#  ADD RULES AFTER THIS LINE
install:
	$(INSTALL) -d -m $(INSTALL_PERMISSIONS) $(wildcard $(ONCRPC)/win32/include/rpc/*.h) $(INSTALL_INCLUDE)/rpc

