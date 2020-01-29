# $FreeBSD: head/audio/Shortwave/Makefile $

PORTNAME=	Shortwave
DISTVERSION=	0.0.1
CATEGORIES=	multimedia

MASTER_SITES=	https://gitlab.gnome.org/World/Shortwave/-/archive/${DISTVERSION}/

MAINTAINER=	segin2005@gmail.com
COMMENT=	GNOME Internet streaming radio player written in Rust

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/COPYING.md

BROKEN=		won't build

BUILD_DEPENDS=	rustc:lang/rust
LIB_DEPENDS=	libhandy-0.0.so:x11-toolkits/libhandy
#RUN_DEPENDS=	ffmpeg:multimedia/ffmpeg

USES=		gettext-tools gnome meson
USE_GNOME=	cairo glib20 gtk30 pango
INSTALLS_ICONS=	yes

GLIB_SCHEMAS=	de.haeckerfelix.Shortwave.gschema.xml

.include <bsd.port.mk>
