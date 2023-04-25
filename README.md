## cobra with viper

`go install github.com/spf13/cobra-cli@latest`

`go mod init github.com/qct-snippets/cobra-example`

`cobra-cli init --author "qct" --license "Apache 2.0" --viper`

`cobra-cli add server`
`cobra-cli add monitor`


rootCmd.PersistentFlags().StringVar(&envVariable, "envVariable", "", "load system environment variable")