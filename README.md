# pbulk-diff-report

1. copy config-sample.pm config.pm
2. Customize config.pm for your need
3.  test with following command 

  PATH=/usr/pkg_bulk/bin:/usr/pkg_bulk/sbin:${PATH} \\  \
  bulkbuild 
  &&
  /usr/pkg_bulk/bin/perl /PATH/TO/perl/pbulk-diff-report > /tmp/mail

4. If above 3 looks good, EITHER

  cat /tmp/mail | /usr/sbin/sendmail -t

  OR

  PATH=/usr/pkg_bulk/bin:/usr/pkg_bulk/sbin:${PATH} \\ \
  bulkbuild
  &&
  /usr/pkg_bulk/bin/perl /PATH/TO/perl/pbulk-diff-report | /usr/sbin/sendmail -t
 
