.include <src.opts.mk>

PACKAGE=	bhyve
FILESDIR=	${SHAREDIR}/bhyve/gdb

.if ${MACHINE_ARCH} == "amd64"
FILES+=		amd64.xml
.endif

.if ${MACHINE} == "arm64"
FILES+=		aarch64-core.xml
.if ${MACHINE_ABI:Mpurecap}
FILES+=		aarch64-capability.xml
.endif
.endif

.include <bsd.prog.mk>
