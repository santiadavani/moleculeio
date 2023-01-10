# moleculeio
MoleculeIO is an application to streamline molecule data lineage between drug hit identification and lead optimization. Key functionality includes:

1. Data management: Users can create, retrieve, update, and search molecules in the database based on attributes like symbols (3 letters or more), IUPAC name, or SMILES string. Platform is designed to be extensible and we can add more attributes as needed.

2. User management: There are three types of users that the platform manages:
    - Unregistered users: These are users without a login. They can browse the existing molecule database and search the DB based on different attributes. This will help your team to share the data without the overhead of creating a login to members outside your team or management.
    - Registered users: These are users with a login and can do everything an unregistered user can do. In addition, they can also create new molecules that can go into the database.
    - Admin users: These are registered users that can approve molecules created by registered users for public view. Admin users functionality can be extended as needed.

3. Machine Learning using SELFIES:  In 2020, there was a [publication](https://iopscience.iop.org/article/10.1088/2632-2153/aba947/pdf) on SELFIES (SELF-referencIng Embedded Strings), a string-based representation of molecules which is 100% robust. This representation is better suited for machine learning workloads. In addition to SMILES representation, we can use SELFIES to recommend new molecules, search molecules in the latent space and predict chemical properties of newly designed molecules.
