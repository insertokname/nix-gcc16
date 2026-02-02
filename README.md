# algol68 gcc 16 

A small hack to build gcc 16, with algol68 support. Currently (02.02.2026) nixpkgs only packages gcc 15 since 16 is still not released. The content of `gcc` is directly taken from [nixpkgs (commit - c3d339e)](https://github.com/NixOS/nixpkgs/tree/c3d339e54cd17d39e929d0b3df5fa7b4d1ace732/pkgs/development/compilers/gcc). 

Some small patches have been applied:
- disabling gcc self checking (`gcc/common/configure-flags.nix`, line 198)
- adding `algol68` as a language inside the configure flags (`gcc/common/configure-flags.nix`, line 222) 
- adding version 16 (`gcc/versions.nix`)