Redis basic

file description

0. Create a Cache class. In the __init__ method, store an instance of the Redis client as a private variable named _redis (using redis.Redis()) and flush the instance using flushdb
1. Redis only allows to store string, bytes and numbers (and lists thereof). Whatever you store as single elements, it will be returned as a byte string. Hence if you store "a" as a UTF-8 string, it will be returned as b"a" when retrieved from the server.
2. Familiarize yourself with the INCR command and its python equivalent
3. Familiarize yourself with redis commands RPUSH, LPUSH, LRANGE, etc.
4. In this tasks, we will implement a replay function to display the history of calls of a particular function
5. In this tasks, we will implement a get_page function (prototype: def get_page(url: str) -> str:). The core of the function is very simple. It uses the requests module to obtain the HTML content of a particular URL and returns it
