# asz80 8080 and 8085 patches

These are patches to asz80 from [asxxxx](http://shop-pdp.net/ashtml/asxxxx.php) to restrict the instruction set to that of the 8080 while still retaining the Z80 opcodes. This is done by adding a directive .8080.

The directive .8085 in addition to restricting to the 8080 instruction set, adds support for the RIM and SIM instructions as well as 8085 undocumented opcodes. See the end of t808x.asm for the syntax of those instructions.

You will need to convert the line endings of the files in the asz80 directory to Unix convention, using for example dos2unix, before the patch will take. Then apply in the directory with:

patch < 8080.patch

## Versioning

First release November 2019

8085 opcodes January 2021

## Authors

* **Ken Yap**

## License

See the [LICENSE](LICENSE.md) file for license rights and limitations (MIT).
