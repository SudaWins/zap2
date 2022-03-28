# zap2
 {
	// Place your snippets for c here. Each snippet is defined under a snippet name and has a prefix, body and 
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

	"Standard C": {
		"prefix": "!!c",
		"body": [
			"#include <stdio.h>//standard input-output",
			"#include <stdlib.h>//standard libary",
			"#include <locale.h>//para localizar uma linguagem",
			"#include <wchar.h> //para acentuações em geral",
			"",
			"int main(){",
			"	setlocale(LC_ALL, \"Portuguese\");//para aceitar acentuação ç etc",
			"	wprintf(L\"Utilizando caracteres e acentuação da língua portuguesa!\\n\\n\"); //colocar um L antes das aspas",
			"",
			"	system(\"pause\");//Pressione qualquer tecla para continuar. . .",
			"",
			"	return 0 ;",
			"}",
		],
		"description": "C standard snippet"
	},

	"wprintf": {
		"prefix": "wprintf",
		"body": [
			"wprintf(L\"$1\")$2;",
			"$3",
		],
		"description": "printf com acentuação"
	},
}
