eav
===

This Perl module implements an entity-attribute-value](http://en.wikipedia.org/wiki/Entity%E2%80%93attribute%E2%80%93value_model) (EAV) data model on top of many storage backends.

[Reddit](http://www.reddit.com/) is an example of a popular site using an EAV-like data model at some point.

EAV Definitions
===============

* **Entity**.  An entity is a primary data type, such as a user, comment, or post.

* **Attribute**.  Attributes are the columns or key names that reference data values,
such as user.name, comment.text, and post.author.

* **Value**.  Values are the actual data referenced by an attribute, such as "This is awesome." for comment.text.

EAV Advantages
==========

* **Simple, static schema.**  The EAV model only requires two tables, one for storing entities and another
for storing data values.

* **Flexible storage.**  The EAV module can support many backends for data storage, which are listed below.

* **Scalability.**  The simplicity of EAV makes it easy to replicate and distribute data to many servers.

Supported Storage Systems
=========================

**Current**
* Native In-memory
* MySQL

**Planned**
* Memcached
* Microsft SQL Server
* PostgreSQL
* Redis
* Riak
* SQLite









