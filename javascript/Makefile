.PHONY: build
build:
	mkdir -p bin
	rm -f bin/app
	npm run build
	cp meta.json bin/meta.json
	cp app bin/app

.PHONY: run
run:
	docker build -t my_node_tutorial_solution .
	docker run -it --env-file .env my_node_tutorial_solution:latest