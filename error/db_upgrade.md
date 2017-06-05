## 做Flask-Migrate数据库迁移

### 遇到了Target database is not up to date报错、No changes in schema detected报错

Flask-Migrate数据库迁移应用场景:

**比如**

    要对User表增加phone字段，记录每个人手机号，这时候会用到Flask-Migrate，实现对表结构的更改



>参考：[]http://blog.csdn.net/clean_water/article/details/53811879

 >     http://www.jianshu.com/p/032723bb9b05

 >     http://www.crifan.com/flask_migrate_upgrade_database_error_alembic_util_exc_commanderror_cannot_locate_revision_identified_by/