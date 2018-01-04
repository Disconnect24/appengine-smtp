# appengine-smtp
a modern fix to a modern solution...?

# backstory
App Engine standard instances don't allow socket connections unless attacted to a `context`. This library, which is literally `net/smtp` at [commit  541bf9f ](https://github.com/golang/go/tree/541bf9f8ea458560353acf78d940c69f5080750a/src/net/smtp) adds a context and uses the App Engine socket API.