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
# Git Force Pull
```javascript
git fetch --all
git reset --hard origin/development
git pull origin development
```
___
# SQL Query Log (should put right after function)
```javascript
db.OnQueryProcessed(func(event *pg.QueryProcessedEvent) {
	query, err := event.FormattedQuery()
	if err != nil {
		panic(err)
	}
	log.Printf("%s %s", time.Since(event.StartTime), query)
})
```
