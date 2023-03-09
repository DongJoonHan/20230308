# 20230308

## Redmine 다운로드
https://downloads.bitnami.com/files/stacks/redmine/4.2.4-0/bitnami-redmine-4.2.4-0-windows-x64-installer.exe


## Plugin 설치 명령들

### DB Migration (Bitnami의 경우)
다음의 위치로 이동
```
cd apps\redmine\htdocs
```

DB Migration 이동
```
bundle exec rake redmine:plugins:migrate RAILS_ENV=production
```


## OpenJDK
위치: https://github.com/ojdkbuild/ojdkbuild


## Redmine DB 백업
```
mysqldump -uroot -pexample redmine > /var/lib/mysql/DBBackup_$(date  '+%A').dump
```


https://kmin135.blogspot.com/2017/08/bitnami-redmine.html
