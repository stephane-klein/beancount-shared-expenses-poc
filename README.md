# plain text accounting shared expenses based on beancount POC

https://github.com/beancount/beancount/

See also https://github.com/stephane-klein/hledger-shared-expenses-poc  

Repository starting point issue (in French): https://github.com/stephane-klein/backlog/issues/193

```sh
$ pip install -r requirements.txt
```

```
$ bean-check main.journal
```

Edit `main.journal.j2` and then execute:

```
$ ./preprocess.py | bean-format -W 10 > main.journal
```

```
$ fava main.journal
```
