# irc-redis

## How to use?

send message to channel, first arg is `channel name`, the secand is `user name`
```
$ ruby pub.rb rubyonrails apa
```

then push message

```
$ ruby pub.rb rubyonrails apa
hello world
```

subscribe channel
```
$ ruby sub.rb
```

also you can check message in redis-cli
```
$ redis-cli
```

then enter `MONITOR`

```
127.0.0.1:6379> MONITOR
```

```
127.0.0.1:6379> MONITOR
OK
1623254033.896253 [0 127.0.0.1:57163] "publish" "rubyonrails" "{\"user\":\"apa\",\"msg\":\"hello\"}"
```
