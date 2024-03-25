# Rule Engine API Specification

This OpenAPI specification defines the API endpoints for the Rule Engine, a system expert API.

## Installation

To generate server code from this OpenAPI specification, you'll need to install the OpenAPI CLI (OpenAPI Generator). Follow the installation guide provided by OpenAPI:
<div style="text-align: center;">
    <a href="https://openapi-generator.tech/docs/installation/">
        <img src="img/openapi-logo.svg" alt="OpenAPI Logo" style="width: 256px; height: 256px;">
    </a>

 [OpenAPI CLI Installation Guide](https://openapi-generator.tech/docs/installation/)

</div>


## Generating Server Code

Once you have installed the OpenAPI CLI, you can generate server code using the following command:

```bash
openapi-cli generate -i openapi.yaml -g go-gin-server --git-host gitlab.com --git-user-id sixbell --git-repo-id componentes/rule-engine/api -o openapi/
```

**Step-by-step description:**

1. `openapi-cli`: The command-line tool being invoked.
2. `generate`: Specifies that the tool should generate code based on the provided input.
3. `-i openapi.yaml`: Specifies the input file (`openapi.yaml`) containing the OpenAPI specification.
4. `-g go-gin-server`: Specifies the generator to use, in this case, generating a Go server with the Gin framework.
5. `--git-host gitlab.com`: Specifies the Git host where the generated code will be pushed.
6. `--git-user-id sixbell`: Specifies the user ID or username associated with the Git repository.
7. `--git-repo-id componentes/rule-engine/api`: Specifies the repository ID or path where the generated code will be pushed, in the format `organization/project`.
8. `-o openapi/`: Specifies the output directory (`openapi/`) where the generated code will be saved.
