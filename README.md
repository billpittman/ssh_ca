# ssh_ca

This repo allows main to be modifed.  It has a single Action to sign keys submitted in the requests folder.
Requests in the user folder are signed with the ssh_user_ca key, and requests submitted in the host folder are
signed with the ssh_host_ca key.

ssh-ca-repo/
├── requests/
│   ├── user
│   │   └── <username>/
│   │       ├── id_rsa.pub
│   │       └── id_ed25519.pub
│   └── host/
│       └── <hostname>/
│           └── ssh_host_ed25519.pub
├── certs/    ### Signed certificates
├── config/   ### common config files
└── README.md

