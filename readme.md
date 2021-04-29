# grpc+grpcgatewayv1

- 安装protobuf
  ```shell
  brew install protobuf
  # 获其他方法均可，protoc 3版本以上
  ```
- 获取grpcgateway，通过git clone，这里grpcgateway是V1版本
  ```bash
  mkdir -p %GOPATH/src/github.com/grpc-ecosystem
  cd %GOPATH/src/github.com/grpc-ecosystem
  git clone git@github.com:grpc-ecosystem/grpc-gateway.git
  git checkout v1.15.2
  ```
- go install grpcwateway，和swagger
  ```bash
  go install \
      github.com/grpc-ecosystem/grpc-gateway/protoc-gen-grpc-gateway \
      github.com/grpc-ecosystem/grpc-gateway/protoc-gen-swagger
  ```

- 通过本项目，生成protoc-gen-go
  ```shell
  cd $GOPATH/src/github.com/DoOR-Team/protoc-gen-go
  go install
  ```