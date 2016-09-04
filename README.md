# billslimbinaries for linux
# all prebuilt in the heroku environment
#
<!-- DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=14.04
DISTRIB_CODENAME=trusty
DISTRIB_DESCRIPTION="Ubuntu 14.04.4 LTS"
NAME="Ubuntu"
VERSION="14.04.4 LTS, Trusty Tahr"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 14.04.4 LTS"
VERSION_ID="14.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"

 -->

 # binaries required
 # pdftotext FOOLABS="ftp://ftp.foolabs.com/pub/xpdf/#{TAR_NAME}"
 # multiregexparser
 # compareplans
 
 to build
 heroku run bash
  cd /app/tmp; curl ftp://ftp.foolabs.com/pub/xpdf/xpdf-3.04.tar.gz -o xpdf.tar.gz && tar zxvf xpdf.tar.gz && cd xpdf-3.04 && ./configure && make && mv xpdf/pdftotext /app/bin

 
