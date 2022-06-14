##  README
###   rootCmd
```go
package cmd

import(
)

var (
		rootCmd := &cobra.Command{
		}
)

func Execute() error {
	return rootCmd.Execute()
}

func init(){
	rootCmd.PersistentFlags.
	rootCmd.AddCommand()
}
```

