# Hello world!

The first program most of us write in anya programming languages is the Hello world. 
So i find this a good place to start, but there are some hurdles to get over.
 
# Setup 
There are a lot of ways one might write software, different Operating system, different editors, 
different languages and so on. We are going to use Go-lang as our programing language, Visual studio code 
as our text editor and git for version control.

## Installation
Thins can very greatly depending on if you are using Windows, Mac or Linux and i will try to provide 
instructions for all of them. I my self use Ubuntu/Linux, which in my experience makes 
software development easier and a lot of what we will do will be done from a terminal. 
This means that Linux or Mac would be preferable.

### git
Ubuntu
```bash
$ sudo apt install git
 ```
 
Mac, Download and install [here](https://git-scm.com/download/mac)

Windows, Download and install [here](https://git-scm.com/download/mac)

### go lang
General documentation on how to install [here](https://golang.org/doc/install)

Ubuntu
```bash
$ sudo apt install golang
 ```
 
Mac, Download and install this [.pkg](https://dl.google.com/go/go1.10.1.darwin-amd64.pkg)

Windows, Download and install this [.msi](https://dl.google.com/go/go1.10.1.windows-amd64.msi)


### Visual Studio Code
Go to [code.visualstudio.com](https://code.visualstudio.com/), download and install



## Create an account on github and fork the project
Since much of the course will be done through git, it is important to have an account to work from
if you want reviews and contribute with your solutions.

* Simply navigate to [github.com](https://github.com/) and sign up for an account.
* Navigate to the project you want to work on. e.g. [github.com/go-hack/hello-world](https://github.com/go-hack/hello-world)
* Now press the "fork" button in the top right corner. This will create a copy, or a fork, of 
  the project on your github account on which you can, change, commit and push code
  

## Cloning and starting work
Now we have everything needed to start working. 

1. Find your go path, a dir named `go` usually located in your home directory. 
1. Navigate and make the following folder structure `$GOPATH/src/github.com/<YOUR GITHUB NAME>`
1. Now run `git clone https://github.com/<YOUR GITHUBHANDLE>/hello-world.git`, this will fetch this 
   project for you to work on 
1. Open Visual Studio Code and select the folder `$GOPATH/src/github.com/<YOUR GITHUB NAME>/hello-world`
   to work from 
   
   
# Lets do some coding

I now assume you have visual studio code open aswell as the project within it. 

1. Let us not begin by creating a folder `students/<YOUR GITHUB NAME>`
1. Now create an empty file within the folder called `main.go`
1. In that file, let us past the following code 
```go
   package main
   
   import "fmt"
   
   func main() {
       fmt.Println("Hello world!")
   }
```

This is your first program written in go. Lets run it.

Navigate to the file in a terminal of command prompt and run the following 

```bash
$ go run main.go
```
 
`Hello world!` should now ampere on your screen 

You can now "save" this to github by running
```bash
$ git add -A
$ git commit -m "My first commit on my first go project"
$ git push
```
