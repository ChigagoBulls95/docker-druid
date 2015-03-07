FROM mysql:5.6

#Same as stock mysql but UTF8. See: https://github.com/docker-library/mysql/pull/14
RUN { \
  echo '[client]'; \
  echo 'default-character-set=utf8';\

  echo '[mysql]'; \
  echo 'default-character-set=utf8'; \

  echo '[mysqld]'; \
  echo 'collation-server = utf8_unicode_ci'; \
  echo "init-connect='SET NAMES utf8'"; \
  echo 'character-set-server = utf8'; \
    
} > /etc/mysql/conf.d/charset.cnf