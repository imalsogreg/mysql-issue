# Reproduce issue 1820

```
[greghale@michelangelo:~/code/mysql-issue]$ nix build
warning: Using saved setting for 'allow-import-from-derivation = true' from ~/.local/share/nix/trusted-settings.json.
warning: Using saved setting for 'extra-substituters = https://cache.iog.io' from ~/.local/share/nix/trusted-settings.json.
warning: Using saved setting for 'extra-trusted-public-keys = hydra.iohk.io:f/Ea+s+dFdN+3Y/G+FDgSq+a5NEWhJGzdjvKNGv0/EQ=' from ~/.local/share/nix/trusted-settings.json.
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
trace: No index state specified for haskell-project, using the latest index state that we know about (2022-08-05T00:00:00Z)!
error: builder for '/nix/store/aycdqc9y9djx5hd2jh2rasqyvglmidz4-mysql-lib-mysql-0.2.1.drv' failed with exit code 1;
       last 10 log lines:
       > unpacking source archive /nix/store/p6802gb80g4sc9ppw2vs9am6pcrf0lsy-mysql-0.2.1.tar.gz
       > source root is mysql-0.2.1
       > setting SOURCE_DATE_EPOCH to timestamp 1634749183 of file mysql-0.2.1/ChangeLog.md
       > patching sources
       > configuring
       > Configure flags:
       > --prefix=/nix/store/p5ikzhlmp21xgky80mabdsm9dn00kkhq-mysql-lib-mysql-0.2.1 lib:mysql --package-db=clear --package-db=/nix/store/57zklj93sxkci3d8yvqvcmaqhd8y6gs8-mysql-lib-mysql-0.2.1-config/lib/ghc-8.10.7/package.conf.d --flags=-developer --exact-configuration --dependency=bytestring=bytestring-0.10.12.0-BvIZHiOJL8O7XxUygqQkmw --dependency=containers=containers-0.6.5.1-EiES0HFUZ8PBGNrpVjoYRF --dependency=array=array-0.5.4.0 --dependency=base=base-4.14.3.0 --dependency=deepseq=deepseq-1.4.4.0 --dependency=ghc-boot-th=ghc-boot-th-8.10.7 --dependency=ghc-prim=ghc-prim-0.6.1 --dependency=integer-gmp=integer-gmp-1.0.3.0 --dependency=pretty=pretty-1.1.3.6 --dependency=rts=rts --dependency=template-haskell=template-haskell-2.16.0.0 --with-ghc=ghc --with-ghc-pkg=ghc-pkg --with-hsc2hs=hsc2hs --with-gcc=cc --with-ld=ld.gold --ghc-option=-optl-fuse-ld=gold --ld-option=-fuse-ld=gold --with-ar=ar --with-strip=strip --disable-executable-stripping --disable-library-stripping --disable-library-profiling --disable-profiling --enable-static --enable-shared --disable-coverage --enable-library-for-ghci --datadir=/nix/store/xrvs50shr8yfd3548q4hwa58sg4as4ld-mysql-lib-mysql-0.2.1-data/share/ghc-8.10.7 --enable-split-sections
       > Configuring library for mysql-0.2.1..
       > Setup: The program 'mysql_config' is required but it could not be found
       >
       For full logs, run 'nix log /nix/store/aycdqc9y9djx5hd2jh2rasqyvglmidz4-mysql-lib-mysql-0.2.1.drv'.
error: 1 dependencies of derivation '/nix/store/g7nfc181q4kjgsfwkpjwrm9rjrw86h6p-mysql-simple-lib-mysql-simple-0.4.8.1-config.drv' failed to build
error: 1 dependencies of derivation '/nix/store/i03jmsibycx7af1g46yg9v6cmjxpaz9j-mysql-simple-lib-mysql-simple-0.4.8.1.drv' failed to build
error: 1 dependencies of derivation '/nix/store/wa5nwyc7x0lfa8wvv3gaywdlhzl70qkv-hello-exe-hello-1.0.0.2.drv' failed to build
```
