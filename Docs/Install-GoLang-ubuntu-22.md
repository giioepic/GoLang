# Ubuntu install golang
```
sudo apt install golang-go
```
```
which go
```
```
echo 'export PATH=$PATH:/usr/bin/go' | sudo tee -a /etc/profile
```
```
source .profile
```
```
go version
```
```
cd ~
mkdir Go-Frist
cd Go-Frist/
go mod init Go-Frist
```
```
vim one.go
```
```
package main

func main() {
	println("Hello World!")
}
```
```
go run one.go
```
