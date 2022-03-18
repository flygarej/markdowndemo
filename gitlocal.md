This repo is just to contain a few diagrams

A repo after a few commits. HEAD points at last commit.
```mermaid
  graph LR
      A(Commit m:0)-->B(Commit m:1);
      B-->C(Commit m:2);
      D(HEAD m)-->C;
```

Adding one more commit updates HEAD to point at latest

```mermaid
  graph LR
      A(Commit m:0)-->B(Commit m:1);
      B-->C(Commit m:2);
      C-->D(Commit m:3)
      E(HEAD m)-->D;
```

Branching from main:HEAD

```mermaid
  graph LR
      A(Commit m:0)-->B(Commit m:1);
      B-->C(Commit m:2);
      C-->D(Commit m:3)
      D-->E(Commit m:4)
      F(HEAD m)-->E;
      D-->G(Commit b1:1)
      G-->H(Commit b1:2)
      I(HEAD b1)-->H
```

Merging from HEAD b1 to main


```mermaid
  graph LR
      A(Commit m:0)-->B(Commit m:1);
      B-->C(Commit m:2);
      C-->D(Commit m:3);
      D-->E(Commit m:4);
      D-->G(Commit b1:1);
      G-->H(Commit b1:2);
      I(HEAD b1)-->H;
      E-->J(Commit m:5);
      H-->J;
      F(HEAD m)-->J;
```

After removing branch 1
```mermaid
  graph LR
      A(Commit m:0)-->B(Commit m:1);
      B-->C(Commit m:2);
      C-->D(Commit m:3);
      D-->E(Commit m:4);
      E-->J(Commit m:5);
      F(HEAD m)-->J;
```
