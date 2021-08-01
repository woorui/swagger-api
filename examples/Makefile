PROTO_FILES=$(shell find ./helloworld -name *.proto)

.PHONY: helloworld
# generate helloworld proto
helloworld:
	protoc --proto_path=./helloworld \
                --proto_path=../third_party \
                --go_out=paths=source_relative:./helloworld \
				--go-grpc_out=paths=source_relative:./helloworld \
				--go-http_out=paths=source_relative:./helloworld \
                ${PROTO_FILES}