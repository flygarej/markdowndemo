Normal workflow is either to clone an existing repo, do work, then pull + push to remote.
Missing in diagram below is adding the remote to the new local repo.)
```mermaid
  flowchart LR;
    A[New directory]-->B[git init .];
    R1[(.git created)]-->B;
    B-->C[edit];
    C-->D[git add .];
    D-->E[git commit -m msg];
    E-->C;
    E-->F[git remote add <remote> URL];
    F-->G[git push remote branch];
    G-->R2[(remote git repo)];
```




Git can be used to sync with two different remotes, using pull/fetch and push.
Branches can also be used to track work done on each end.

```mermaid
  flowchart LR;
  A[Remote repo A]<-->B[Local repo in .git];
  B<-->C[Remote repo B];
```
