Ranch TCP Reverse
=================

This example uses a gen_server to handle a protocol to revese input. See
reverse_protocol.erl for the implementation, and documentation at
the following URL:

http://ninenines.eu/docs/en/ranch/HEAD/guide/protocols/#using_gen_server

To build the example:
``` bash
$ make
```

To start the release in the foreground:

``` bash
$ ./_rel/bin/tcp_reverse_example console
```

Then start a telnet session to port 5555:
``` bash
$ telnet localhost 5555
```

Type in a few words and see them reversed! Amazing!

Be aware that there is a timeout of 5 seconds without receiving
data before the example server disconnects your session.