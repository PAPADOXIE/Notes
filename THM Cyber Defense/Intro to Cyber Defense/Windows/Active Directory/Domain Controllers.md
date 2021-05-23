## Domain Controllers
Windows server which has Active Directory Domain Services installed on it
- Holds the AD DS data store
- Handles authentication and authorization services
- Replicates updates from other domain controllers in the forest
- Allows admin access to manage domain resources

### AD DS Data Store
Stores the databases and processes needed to store and manage directory information.
- Contains the NTDS.dit
- Stored in `%SystemRoot%\NDTS`
- Accessible only by the domain controller