# Created by: Mattis Michel <sic_zer0@hotmail.com>
# $FreeBSD: head/x11-wm/matwm2/Makefile 517000 2019-11-07 18:36:55Z zeising $

PORTNAME=	matwm2
DISTVERSION=	0.1.2pre3
CATEGORIES=	x11-wm

USE_GITHUB=	yes
GH_ACCOUNT=	segin

MAINTAINER=	sic_zer0@hotmail.com
COMMENT=	Minimalistic, yet functional window manager for X11

LICENSE=	MIT

HAS_CONFIGURE=	yes
CONFIGURE_ARGS=	--cc=${CC} --prefix=${PREFIX} --mandir=${MANPREFIX}/man
USES=		xorg
USE_XORG=	x11 xext xinerama xft

PLIST_FILES=	bin/matwm2 man/man1/${PORTNAME}.1.gz

post-extract:
	@${RM} -rf ${WRKSRC}/clockreset ${WRKSRC}/hemorrhage ${WRKSRc}/matirc2 ${WRKSRC}/minix-ports ${WRKSRC}/readbin ${WRKSRC}/deskpaint ${WRKSRC}/keygrab ${WRKSRC}/matserve ${WRKSRC}/netmsg-c ${WRKSRC}/readpe ${WRKSRC}/fbstring ${WRKSRC}/kshell ${WRKSRC}/netmsg-fb ${WRKSRC}/sed ${WRKSRC}/freebsd-utils ${WRKSRC}/longview ${WRKSRC}/md5sum ${WRKSRC}/quirky-x11-hacks ${WRKSRC}/sto
	@${MV} ${WRKSRC}/matwm2/* ${WRKSRC}/
	@${RM} -rf ${WRKSRC}/matwm2/

.include <bsd.port.mk>
