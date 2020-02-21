# snippets-vscode
Snippets para automatizar rotinas repetitivas no eproc

```json
  {
	// Place your snippets for php here. Each snippet is defined under a snippet name and has a prefix, body and
	// description. The prefix is what is used to trigger the snippet and the body will be expanded and inserted. Possible variables are:
	// $1, $2 for tab stops, $0 for the final cursor position, and ${1:label}, ${2:another} for placeholders. Placeholders with the
	// same ids are connected.
	// Example:
	// "Print to console": {
	// 	"prefix": "log",
	// 	"body": [
	// 		"console.log('$1');",
	// 		"$2"
	// 	],
	// 	"description": "Log output to console"
	// }

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
