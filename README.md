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
# Fix swag not found even downloaded from github.com/swaggo/swag/cmd/swag
```javascript
export GOPATH=$PATH:$(go env GOPATH)/binROOT=`
```
___
# Git Force Pull
```javascript
git fetch --all
git reset --hard origin/development
git pull origin development
```
___
# SQL Query Log
```javascript
db.OnQueryProcessed(func(event *pg.QueryProcessedEvent) {
	query, err := event.FormattedQuery()
	if err != nil {
		panic(err)
	}
	log.Printf("%s %s", time.Since(event.StartTime), query)
})
```
___
# Regex to find a string:
```javascript
.*?
```
