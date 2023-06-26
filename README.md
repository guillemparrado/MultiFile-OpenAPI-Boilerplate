
# Multi-File OpenAPI boilerplate

A starter template for **OpenAPI Specification** (OAS) projects.

This project splits the [Swagger Petstore](https://petstore.swagger.io/) example from the official documentation into smaller files. It also adds handy commands to build, lint, and preview the OpenAPI document from the terminal.

You can use this template to guide the organization of your project. Either if you want to create a new OpenAPI document from scratch or if you already have it defined. 

## Features

* 📝 Write OpenAPI definitions in different files.
* 🔀 Combine all files with [APIDevTools/swagger-cli](https://github.com/APIDevTools/swagger-cli).
* ✅ Validate and lint the OpenAPI document with [stoplight/spectral](https://github.com/stoplight/spectral).
* ~~✨ Publish reference docs with [redocly/redoc](https://github.com/Redocly/redoc) & GitHub Pages.~~ (simplified on this fork)

## Why?

When I used to document APIs following the OpenAPI spec, I always ended up with documents of thousands of lines, which were a nightmare to maintain.

For this reason, I explored how to split OpenAPI documents. Jump over to my [blog](https://davidgarcia.dev/posts/how-to-split-open-api-spec-into-multiple-files/) to learn more about the process. Based on my research, I created this opinionated template to define, test, and publish modular OpenAPI projects.

Properly organizing your project comes with great advantages. By splitting a large OpenAPI spec into multiple files, it will not only be much easier to handle. Documenting it will be much more enjoyable, too. I also regularly get the feedback that other developers are more willing to contribute and propose changes to the document with this structure.

## Getting started

### Requirements

* Node.js 16 (current)

### Installation

1. Clone the repository.

    ```
    git clone https://github.com/dgarcia360/openapi-boilerplate.git
    ```

2. Install the project dependencies.

    ```
    npm install
    ```

3. Edit `openapi.yaml` to fit your API definition. If you’re not familiar with the OpenAPI Specification, read [Getting started with OAS](https://swagger.io/solutions/getting-started-with-oas/) first.

## Useful commands

The project will build, lint, and preview the OpenAPI document from the terminal, with the following commands:

### Build

The command bundles the spec as one `.yaml` file.

```
npm run build
```

The minified document is stored in `_build/openapi.yaml`.

### Test

The command checks if the document follows the OpenAPI 3.0 Specification.

```
npm run test
```


