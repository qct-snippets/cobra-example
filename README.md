## cobra with viper

### Init
`go install github.com/spf13/cobra-cli@latest`

`go mod init github.com/qct-snippets/cobra-example`

`cobra-cli init --author "qct" --license "Apache 2.0" --viper`

`cobra-cli add server`

`cobra-cli add monitor`


### Run
* Run with root command:
```
A longer description that spans multiple lines and likely contains
examples and usage of using your application. For example:

Cobra is a CLI library for Go that empowers applications.
This application is a tool to generate the needed files
to quickly create a Cobra application.

Usage:
  cobra-example [command]

Available Commands:
  completion  Generate the autocompletion script for the specified shell
  help        Help about any command
  monitor     A brief description of your command
  server      A brief description of your command

Flags:
      --config string   config file (default is $HOME/.cobra-example.yaml)
  -h, --help            help for cobra-example
      --key1 string     load system environment variable
  -t, --toggle          Help message for toggle

Use "cobra-example [command] --help" for more information about a command.
```

* Run with env variable:
`ENV_KEY1=2 go run main.go monitor`:
```
Read key1: 2
monitor called
```