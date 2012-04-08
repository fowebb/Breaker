Breaker, a lazy programmer's remote pdb.
==========
Automatically post mortem breaks on any exception, anywhere in your
(or others'...) code, and launches an rdb session
(credit to celery.contrib.rdb), allowing you to connect and poke around.

Just add this line at import time:
<pre><code>import breaker</pre></code>

When an exception is hit, you are greeted with:

<pre><code>
Remote Debugger:6900: Please telnet 127.0.0.1 6900.  Type `exit` in session to continue.
Remote Debugger:6900: Waiting for client...
</pre></code>

Combine this with pdb++'s sticky lines to get a great picture of where your code crapped its pants.
