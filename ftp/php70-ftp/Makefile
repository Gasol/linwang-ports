# Created by: Alex Dupre <ale@FreeBSD.org>
# $FreeBSD: head/ftp/php70-ftp/Makefile 422569 2016-09-21 15:43:47Z tz $

CATEGORIES=	ftp

MASTERDIR=	${.CURDIR}/../../lang/php70

PKGNAMESUFFIX=	-ftp

post-patch:
	@${REINPLACE_CMD} s/HAVE_OPENSSL_EXT/__FreeBSD__/ \
		${WRKSRC}/ftp.* ${WRKSRC}/php_ftp.*

.include "${MASTERDIR}/Makefile"
