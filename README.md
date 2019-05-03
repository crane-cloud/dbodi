# Kubernetes Management Dashboard

A custom Graphical User Interface (GUI) layer that directly interfaces with the Kubernetes API. More specifically, the GUI will be used to:

* Create unique namespaces for organizational categories where required on the different clusters for example based on teams such as development, production and testing. This will allow clients to logically separate concerns while ensuring Continuous Integration and Continuous Delivery (CI/CD) of services.

* Deploy and manage containerised applications (deployment, scalability and cluster data replication). This will help clients to easily manage their applications using an intuitive interface with no need to master and interface with the command line interface of a UNIX-based system.

* Manage external access to cluster services with possible load balancing definitions such as ingress and DNS. Services defined in the cluster require external access and this is challenging especially in bare metal environments. A combination of DNS, ingress and popular load balancing solutions will be further explored and findings used to inform the approach.

* A web-based Command Line Interface (CLI) to interact with k8s API for user application specific information - For users proficient with UNIX-based terminals, controlled CLI access will be provided via the dashboard to support Kubernetes control commands restricted to the
client namespace(s).

User management with support for delegation of roles to users.

* With Role-Based Access Control (RBAC) integrated to later Kubernetes versions, this will act as a building block for managing cluster resources by users. A highly available user database will be deployed as a microservice to the cluster for access, and client administrators should be able to delegate roles to users.

* Other account management features such as creation of accounts, account activation/deactivation, password resets shall be provided and effected from the GUI.

* Testing accounts shall be default on creation of an account on the platform. This provides a limited environment where users can experiment with most of the system features with possible upgrade to paid deployment plans with full functionality.
