andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2$ git clone 
git@github.com:hhru/frontik.git

Cloning into 'frontik'...

remote: Counting objects: 7572, done.

remote: Compressing objects: 100% (2486/2486), done.

remote: Total 7572 (delta 5037), reused 7543 (delta 5015)

Receiving objects: 100% (7572/7572), 1.87 MiB | 397.00 KiB/s, done.

Resolving deltas: 100% (5037/5037), done.

Checking connectivity... done.



andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2$ cd frontik/

andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2/frontik$ git clone . A

Cloning into 'A'...

done.

andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2/frontik$ git clone . B

Cloning into 'B'...

done.

andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2/frontik$ cd B

andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2/frontik/B$ git filter-
branch  --tree-filter 'rm -rf frontik/testing'

Rewrite 445a2f8c85420bca45b3b8a76ec20c9153097635 (639/1168)error: 

duplicate parent 6deb00cfd2c81405715ee0a9a9c39f0ed78785a7 ignored

Rewrite 8d43cda5783bee8b4cc8d9c3374b262f68dbba73 (1168/1168)

Ref 'refs/heads/master' was rewritten

andrew@HP-ENVY-m6-Notebook-PC:~/Desktop/hh/git/lab2/frontik/B$ cd ../A

git filter-branch --subdirectory-filter "./frontik/testing" -- --all
