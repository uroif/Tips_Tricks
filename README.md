## Tips
___
# Set $GOPATH and $GOROOT
Set GOPATH
```javascript
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
```
Set GOROOT
```javascript
export GOROOT=$HOME/go/src
export PATH=$PATH:$GOROOT/bin
```
Remove GOROOT
```javascript
export GOROOT=`
```
___
Fix "swag: command not found" even downloaded from github.com/swaggo/swag/cmd/swag
```javascript
PATH=$PATH:$(go env GOPATH)/bin
```
___
# Git Force Pull
```javascript
git fetch --all
git reset --hard origin/development
git pull origin development
```
