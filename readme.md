# grpc+grpcgatewayv1

- 安装protobuf
  ```shell
  brew install protobuf
  # 获其他方法均可，protoc 3版本以上
  ```
- 获取grpcgateway，通过git clone，这里grpcgateway是V1版本
  ```bash
  go install \
    github.com/grpc-ecosystem/grpc-gateway/protoc-gen-grpc-gateway@v1.15.2 \
    github.com/grpc-ecosystem/grpc-gateway/protoc-gen-swagger@v1.15.2
  ```

- 通过本项目，生成protoc-gen-go
  ```shell
  cd $GOPATH/src/github.com/DoOR-Team/protoc-gen-go
  go install
  ```