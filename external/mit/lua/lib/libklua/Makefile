LIB=		klua
SRCS=		lapi.c lauxlib.c lbaselib.c lcode.c ldblib.c ldebug.c ldo.c \
		ldump.c lfunc.c lgc.c linit.c liolib.c llex.c lmathlib.c \
		lmem.c loadlib.c lobject.c lopcodes.c loslib.c lparser.c \
		lstate.c lstring.c lstrlib.c ltable.c ltablib.c ltm.c \
		lundump.c lvm.c lzio.c

.include <bsd.own.mk>

INCS=		lauxlib.h lua.h lua.hpp luaconf.h lualib.h
INCSDIR=	/usr/include

CFLAGS+=	-DLUA_USE_POSIX -DLUA_USE_DLOPEN -D_NOFPA
CWARNFLAGS.clang+=	-Wno-empty-body

.PATH:		${NETBSDSRCDIR}/external/mit/lua/dist/etc
.PATH:		${NETBSDSRCDIR}/external/mit/lua/dist/src

.include <bsd.lib.mk>
