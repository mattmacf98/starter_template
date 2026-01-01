.PHONY: build
build:
	mkdir -p bin
	rm -f bin/app
	go build -o bin/app main.go
	cp meta.json bin/meta.json

.PHONY: run
run:
	make build
	docker build -t my_cli_tutorial_solution .
	docker run -it --env-file .env my_cli_tutorial_solution:latest