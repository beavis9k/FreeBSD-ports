# $FreeBSD$

PORTNAME=	ktp-text-ui
PORTVERSION=	${KTP_VERSION}
PORTREVISION=	5
CATEGORIES=	net-im kde
MASTER_SITES=	KDE/${KTP_BRANCH}/kde-telepathy/${PORTVERSION}/src
PKGNAMESUFFIX=	-kde4

MAINTAINER=	kde@FreeBSD.org
COMMENT=	KDE chat window application

LIB_DEPENDS=	libtelepathy-qt4.so:net-im/telepathy-qt4 \
		libtelepathy-logger-qt4.so:net-im/telepathy-logger-qt4 \
		libktpcommoninternalsprivate.so:net-im/ktp-common-internals-kde4
RUN_DEPENDS=	${KDE_PREFIX}/bin/ktp-contactlist:net-im/ktp-contact-list-kde4

USES=		cmake compiler:c++11-lang gettext kde:4 qt:4 tar:bzip2
USE_KDE=	automoc4
USE_QT=		corelib webkit xml \
		moc_build qmake_build rcc_build uic_build
USE_LDCONFIG=	yes

.include <bsd.port.mk>
