# Admin-Reset-Service
Admin Reset Service

The general idea of this project is to create a windows service which resets the Local Administrator password to a randomly generated one. 

This password will be reset upon the start of the service and also will monitor when the administrator account is used so it can then be reset again when the account is no longer in use.

The randomly generated password should be encrypted using a certicate public key exported from a pki certificate. This encrypted string is then saved to a file or to a database for retrieval.
