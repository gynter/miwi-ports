# Created by: Alex Dupre <ale@FreeBSD.org>
# $FreeBSD: head/ftp/php56-ftp/Makefile 367268 2014-09-04 14:24:25Z ale $

CATEGORIES=	ftp

MASTERDIR=	${.CURDIR}/../../lang/php70

PKGNAMESUFFIX=	-ftp

post-patch:
	@${REINPLACE_CMD} s/HAVE_OPENSSL_EXT/__FreeBSD__/ \
		${WRKSRC}/ftp.* ${WRKSRC}/php_ftp.*

.include "${MASTERDIR}/Makefile"
