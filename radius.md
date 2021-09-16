# Radius Concepts

notes taken from above article at: <https://wiki.freeradius.org/guide/Concepts>

How things work in RADIUS
The client sends the server a RADIUS authentication request. You don't decide what's in the request, the client does. The server doesn't decide what's in the request, the client does. The client is 100% responsible for everything in the request.

Picking an Auth-Type - authorize {}
The radius server looks at the request and says:

Hmmm... can I deal with this request?

The answer to that depends on what authentication types you have enabled in the server, what the server can look up in a database, and what is in the request.

The server will then start querying the modules in the authorize section:

Unix module, can you handle this one?

Pap module, can you handle this one?

Mschap module, can you handle this one?

At some point, one of the modules will say:

Yes, I see something in the request I recognize. I can do something!

The module does this by looking in the request for key attributes, such as MS-CHAP-Challenge (for mschap), or CHAP-Challenge (for chap), or EAP-Message (for eap). Or it may just assume it needs to add something to every request.

If the module thinks it has a shot at authenticating the user it'll say:

I can't authenticate this user now (I was just told to authorize them), but my pal in the Authenticate section can! Hey, set the Auth-Type to me!

If the module doesn't see anything it recognizes, or knows it doesn't need to lookup anything, it does nothing.