# 运行`Post.generate_fake(100)`时总是出现

```python

    Tracevack:
    File"<console>",line 1, in <module>
    NameError:name 'Post' is not defined
```


发现在`manage.py`中

`def make_shell_context():
    return dict(app=app, db=db, User=User, Role=Role, Permission=Permission,
                Post=Post) #右边app是指hello.py中的实例对象，左边app是自己命名，
                                                   #以后可以在命令行中输入，就调用了app实例`

开始的时候没有写`Post=Post`,当我运行`python manage.py shell`时Post.generate_fake(100),不能调用Post实例