# DNS-Server that implements recursive and iterative communication

A command line Project which helps to understand how the DNS servers communicate with each other.

# Setup

Fork and Clone OR Clone directly the project. And then follow these below steps.

This project makes use of [dnspython](https://github.com/rthalley/dnspython) library.
Install `dnspython` library:

```bash
pip install dnspython
```

Run the `servers` on different terminals processes: (Refer setup file)

```bash
python localDnsServer.py
python rootDnsServer.py
python tldDnsServer.py
python authoritativeDnsServer.py
```

Now Run the `client` file:

```bash
python client.py
```

You can give any domain and the servers will give you the respective IP Addresses.

It also uses local cache to store the recently queried domains.
