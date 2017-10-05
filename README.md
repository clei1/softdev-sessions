Cookies & Sessions
Cookies are files that websites will save to your web browser to store information on a local machine.
Useful for keeping track of persistent information like login credentials.

Sessions
Flask sessions are securely signed cookies. Since they are encrypted, they cannot be modified by the user of the local machine.
The session object works exactly like a dictionary.
Add data to a session:
session[KEY] = DATA
Remove data from a session:
session.pop(KEY)

In order for Flask to create an encrypted cookie on your computer, you need to provide a key.

<APP>.secret_key = <RANDOM STRING>

good way to get random data : os.urandom(32)
returns 32 random bits of data as a string
never put the secret key in a public place