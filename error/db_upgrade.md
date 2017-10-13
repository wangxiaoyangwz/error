## 做Flask-Migrate数据库迁移

### 遇到了Target database is not up to date报错、No changes in schema detected报错

我解决问题的方法不是很好，等我找到更好的方法后在修改

1. 我将migrate文件删了
2. 我又删除了flasky/data-dev.sqlite文件
3. python manage.py db init
4. python manage.py db migrate -m ''
5. python manage.py upgrade

成功完成，但是数据也都没有了

Flask-Migrate数据库迁移应用场景:

**比如**

    要对User表增加phone字段，记录每个人手机号，这时候会用到Flask-Migrate，实现对表结构的更改



>参考：[1](http://blog.csdn.net/clean_water/article/details/53811879)

 >     [2(]http://www.jianshu.com/p/032723bb9b05)

 >     [3] (http://www.crifan.com/flask_migrate_upgrade_database_error_alembic_util_exc_commanderror_cannot_locate_revision_identified_by/)
