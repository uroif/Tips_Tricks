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
# For error "No operations defined in spec!"
```
> Add comment above functions in controllers folder
> Run swag init command
```
