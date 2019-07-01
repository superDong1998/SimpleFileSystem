# SimpleFileSystem

Software Engineering Operating System Project of File System

#implementation------------------------------------------------------------
# Design

To implement Filesystem::debug, you will need to load the file system
data structures and report the superblock and inodes.

How will you read the superblock?
How will you traverse all the inodes?
How will you determine all the information related to an inode?
How will you determine all the blocks related to an inode?

Response.

To implement FileSystem::format, you will need to write the superblock
and clear the remaining blocks in the file system.

What pre-condition must be true before this operation can succeed?
What information must be written into the superblock?
How would you clear all the remaining blocks?

Response.

To implement FileSystem::mount, you will need to prepare a filesystem
for use by reading the superblock and allocating the free block bitmap.

What pre-condition must be true before this operation can succeed?
What sanity checks must you perform?
How will you record that you mounted a disk?
How will you determine which blocks are free?

Response.

To implement FileSystem::create, you will need to locate a free inode
and save a new inode into the inode table.

How will you locate a free inode?
What information would you see in a new inode?
How will you record this new inode?

Response.

To implement FileSystem::remove, you will need to locate the inode and
then free its associated blocks.

How will you determine if the specified inode is valid?
How will you free the direct blocks?
How will you free the indirect blocks?
How will you update the inode table?

Response.

To implement FileSystem::stat, you will need to locate the inode and
return its size.

How will you determine if the specified inode is valid?
How will you determine the inode's size?

Response.

To implement FileSystem::read, you will need to locate the inode and
copy data from appropriate blocks to the user-specified data buffer.

How will you determine if the specified inode is valid?
How will you determine which block to read from?
How will you handle the offset?
How will you copy from a block to the data buffer?

Response.

To implement FileSystem::write, you will need to locate the inode and
copy data the user-specified data buffer to data blocks in the file
system.

How will you determine if the specified inode is valid?
How will you determine which block to write to?
How will you handle the offset?
How will you know if you need a new block?
How will you manage allocating a new block if you need another one?
How will you copy from a block to the data buffer?
How will you update the inode?

# Errata

Describe any known errors, bugs, or deviations from the requirements.

# Extra Credit

Describe what extra credit (if any) that you implemented.
