# Docs are read from a local turborel clone.
# Use `make dev DOCS_LOCAL=` to fetch them from GitHub instead.
DOCS_LOCAL ?= ../turborel
export DOCS_LOCAL

.PHONY: dev serve build clean

dev: node_modules
	npm run dev

serve: node_modules
	npm start

build: node_modules
	npm run build

node_modules: package-lock.json
	npm ci

clean:
	rm -rf _site .cache
