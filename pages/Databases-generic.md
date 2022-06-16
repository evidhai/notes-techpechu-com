- [[Redshift]] - It's a warehouse service
- [[QLDB]] - Quantum Ledge Database
  collapsed:: true
	- It's a ledger based database
	- It's serverless
	- plaintext -> hash -> store it
	- can be integrated with [[Kinesis]]
- [[Document DB]]
  collapsed:: true
	- It's non relational DB
	- It's document based database
	- Endpoints
		- Cluster
			- points to the current primary DB
		- Reader Endpoints
			- Connects to read replicas
		- Instance
			- It's direct instances for specific purpose to serve traffic directly
- [[DMS]] - Database migration service
  collapsed:: true
	- Its service to migrate data from one to other database by transferring the data in right format
- [[keyspaces]]
	- It's compatible with casandra
	- Can be queries with Casandra Query language (CQL)
	-