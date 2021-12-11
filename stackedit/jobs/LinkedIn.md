# Craftmanship / Design

## Tradeoffs and edgecases

Design of the CDN:

* Continue to serve traffic even if it be comes disconnect from the rest of network
* Content may be stale but in most cases it is better than a 404.
* Customers should have configured an expiration, i.e. e-commerce sale
* If the need to update, i.e. relieazed the expiration is set for the wrong timezon, the disconnect PoP would not get the new configs. This is an edge case were could be serving the wrong conent, but tradeoff to provide a better experince for most of our customers' customers.

## Performance, Complexity vs Simplicity

Python + Functional

* Python is quick for me to make a library or cli
* Most application I write are not performance bound
* I prefer to use function paradigms w/ Python for data integrity
* Network I/O is a freque
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTQ4OTIwNTk1MiwxMjU2MzY3NTg5XX0=
-->