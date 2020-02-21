# snippets-vscode
Snippets para automatizar rotinas repetitivas no eproc

```json
  {
	"Dump or die": {
		"prefix": "ddd",
		"body": [
			"var_dump($1) or die();"
		],
		"description": "Var Dump"
	},

	"DTO": {
		"prefix": "dto",
		"body": [
			"\\$obj$1DTO = new $1DTO();",
			"\\$obj$1DTO->$0"
		],
		"description": "DTO Create"
	},

	"RN Listar": {
		"prefix": "rn:listar",
		"body": [
			"\\$obj$1DTO = new $1DTO();",
			"\\$obj$1DTO->$0",
			"\n",
			"\\$obj$1DTO = new $1();",
			"\\$obj$1DTO = \\$obj$1RN->listar(\\$obj$1DTO);",
			"return \\$obj$1DTO;"

		],
		"description": "RN listar Create"
	},

	"RN Consultar": {
		"prefix": "rn:consultar",
		"body": [
			"\\$obj$1DTO = new $1DTO();",
			"\\$obj$1DTO->$0",
			"\n",
			"\\$obj$1DTO = new $1();",
			"\\$arr$1DTO = \\$obj$1RN->consultar(\\$obj$1DTO);",
			"return \\$arr$1DTO;"
		],
		"description": "RN consultar Create"
	},

	"RN Cadastrar": {
		"prefix": "rn:cadastar",
		"body": [
			"\\$obj$1DTO = new $1DTO();",
			"\\$obj$1DTO->$0",
			"\n",
			"\\$obj$1DTO = new $1();",
			"\\$obj$1DTO = cadastrar(\\$$1);"
		],
		"description": "RN Cadastrar Create"
	},

	"RN Alterar": {
		"prefix": "rn:alterar",
		"body": [
			"\\$obj$1DTO = new $1DTO();",
			"\\$obj$1DTO->$0",
			"\n",
			"\\$obj$1DTO = new $1();",
			"\\$obj$1DTO = alterar(\\$$1);"
		],
		"description": "RN alterar Create"
	}


}
```
