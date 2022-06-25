# Brew Install GoLang
```
brew upgrade
brew update && brew install golang
```
```
mkdir -p $HOME/go/{bin,src,pkg}
```
# edit ~/.zshrc and put following line
```
export GOPATH=$HOME/go
export GOROOT="$(brew --prefix golang)/libexec"
export PATH="$PATH:${GOPATH}/bin:${GOROOT}/bin"
```
```
source $HOME/.zshrc
```
# Install gvm
```
zsh < <(curl -s -S -L https://raw.githubusercontent.com/moovweb/gvm/master/binscripts/gvm-installer)
source /Users/ziyiouyang/.gvm/scripts/gvm
```
```
gvm listall
```
# Write your first go program name main.go with following content, and put it under $HOME/go/src/hello
```
package main

func main() {
	println("Hello World!")
}
```
##### Then run it with following command:
```
go run main.go
```
