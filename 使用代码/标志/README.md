##  README
修饰命令的 行为
在使用上是 可选的 

###   全局设置persistent
对command和子command都有效
```shell
var Verbose bool
rootCmd.PersistentFlags().BoolVarP(&Verbose, "verbose", "v", false, "verbose output")
```



###   局部设置local
```shell
var Source string
rootCmd.Flags().StringVarP(&Source, "source", "s", "", "Source directory to read from")
```


###   把可选转化成必选
```shell
var Name string
rootCmd.Flags().StringVarP(&Name, "name", "n", "", "user name (required)")
rootCmd.MarkFlagRequired("name")
```

