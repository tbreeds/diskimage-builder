===================
partitioning-parted
===================
Sets up a partitioned disk using parted, according to user needs.

Environment Variables
---------------------
DIB_PARTITIONING_PARTED_SCHEMA
  : Required: Yes
  : Default: mklabel gpt
             mkpart primary 0% 100%
  : Description: A multi-line string specifying a disk schema in sectors.
  : Example: ``DIB_PARTITIONING_SFDISK_SCHEMA="
    mklabel gpt
    mkpart primary 0% 100%
    " will create a gpt disk lable with a single partition filling the disk.
