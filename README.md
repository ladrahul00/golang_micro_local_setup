# golang_micro_local_setup

1. To fix etcd issue as the grpc >= v1.26.0, <1.27.1 has issues probably
  https://github.com/etcd-io/etcd/issues/11931
  Fix: `go get google.golang.org/grpc@v1.26.0`
  
  
  
2. To include private repo imports
  go env -w GOPRIVATE="github.com/wolf00/*"
  
3. ssh config for multiple ssh keys
  ```
    Host github.com
      HostName github.com
      User git
      IdentityFile ~/.ssh/id_rsa_github

    Host unscrambl.com
        HostName unscrambl.com
        User rahullad
        IdentityFile ~/.ssh/id_rsa
  ```
 
