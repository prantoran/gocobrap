

- user [cobra generator](https://github.com/spf13/cobra/blob/master/cobra/README.md) is used to auto-generate bare main.go and rootCmd file
    - $ cobra init github.com/prantoran/gocbrap/cobrago // cobrago must not initially exist

- adding commands
    - goto cobrago dir
    - $ cobra add root 
    - $ cobra add add                 // app add
    - $ cobra add config                // app config
    - $ cobra add create -p 'configCmd' // app config create

- executing
    - go run main.go add
    - go run main.go config
    - go run main.go config create
    - go run main.go help add
    - go run main.go -a "pinku" --config `pwd`/.cobra.yaml add
- You will additionally define flags and handle configuration in your init() function.



* Note:
    - use camelCase for command names.

remit
gemit