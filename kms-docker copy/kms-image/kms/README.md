# keywords-management-backend

## 1. 克隆到本地
```
    git clone https://github.com/whsasf/keywords-management-backend.git
```
## 2. 安装依赖, 确保python >=3.6 ,建议在 virtualenv 等虚拟环境中开发
```
    pip3 install -r requirements.txt
```
## 3. 确保mongodb 已经启动(port:27017)
## 4. 本地启动：
```
    uvicorn main:app --reload --port 3000  --host 0.0.0.0
```
## 5. 测试
   所有测试用例在test目录下。目前只写了Account相关的测试，供其他测试可以参考。使用fastAPI深度集成的Pytest。测试前请确保pytest已经安装
   ```
   pip3 install pytest
   ```
   然后，在根目录下运行
   ```
    pytest --disable-warnings  -vv
   ```