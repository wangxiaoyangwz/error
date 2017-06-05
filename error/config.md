```python
    config={#config字典注册了不同配置环境
        'development':DevelopmentConfig,
        'testing':TestingConfig,
        'production': ProductionConfig,

        'default':DevelopmentConfig#注册默认配置，开发环境
}
```

注意一定要有逗号