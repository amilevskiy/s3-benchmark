#

PORTNAME=	s3-benchmark
PORTVERSION=	0.0.4
DISTVERSIONPREFIX=	v
CATEGORIES=	local net

MAINTAINER=	none@FreeBSD.org
COMMENT=	Measure Amazon S3's performance
WWW=		https://github.com/${GH_ACCOUNT}/${PORTNAME}

LICENSE=	MIT
LICENSE_FILE=	${WRKSRC}/LICENSE

USES=		go:modules

USE_GITHUB=	yes
GH_ACCOUNT=	amilevskiy

PLIST_FILES=	bin/${PORTNAME}

GO_BUILDFLAGS+=	-ldflags="-s -w -X 'main.version=${DISTVERSIONPREFIX}${PORTVERSION}'"

.include "${.CURDIR}/Makefile.deps"

.include <bsd.port.mk>
