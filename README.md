项目根目录: heibbs/
├── pom.xml                  # 父POM，统一管理版本和依赖
├── heibbs-common/           # 公共模块，存放各模块共享代码
├── heibbs-core/             # 核心业务模块，包含服务和数据访问
├── heibbs-api/              # API接口模块，定义前后端交互接口
├── heibbs-frontend/         # 前端模块(用户端)
├── heibbs-admin/            # 管理端模块(后台管理)
└── heibbs-boot/             # 启动模块，包含Spring Boot主类

# 各模块职责说明:
1. heibbs-common:
    - 通用工具类、常量定义
    - 全局异常处理、通用响应体
    - 公共实体类、枚举
    - 安全相关基础配置

2. heibbs-core:
    - 业务逻辑层(service)
    - 数据访问层(repository/mapper)
    - 领域模型(entity)
    - 第三方服务集成

3. heibbs-api:
    - 控制器(controller)
    - 请求参数验证
    - 接口文档配置(Swagger/SpringDoc)
    - 前后端交互DTO

4. heibbs-frontend:
    - 用户端页面和资源
    - 前端路由和状态管理
    - 前端与API交互逻辑

5. heibbs-admin:
    - 管理后台页面和资源
    - 管理端特有业务逻辑
    - 权限管理相关功能

6. heibbs-boot:
    - Spring Boot启动类
    - 主配置文件(application.yml)
    - 外部化配置管理
