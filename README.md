# go-up_examples

## Example usage of go-up

Before Go-Up, I used to use [Viper](https://github.com/spf13/viper). 
Viper is great and I surely recommend it; nevertheless, all of its features are not for free. In fact, it adds tons of dependencies that make the application much heavier.

So, if like me you aspire to code which is as light as possible and you can live with a smaller set of features (BWT go-up has some unique aces in the hole like recursive placeholders resolution!), then you should probably take into account a lighter alternative like go-up.

To show the impact that a single library can have on your application, I created three small examples, these are:

- *go-up* : a Go application that, using **go-up**, reads "Hello World" from a config file and prints it
- *plain* : a Go application that prints "Hello World"
- *viper* : a Go application that, using **viper**, reads "Hello World" from a config file and prints it

When built, they produce surprising results:

| Library       | Produced Binary Size |
| ------------- |---------------------:|
| Go-Up         |             2.185 KB |
| Plain Go      |             2.000 KB |
| Viper         |            11.782 KB |

<ins>The Viper based binary file is nearly 6 times bigger than the other implementations!</ins>

(Build performed with go1.13 linux/amd64 on Ubuntu 18.04)
