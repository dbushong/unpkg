Overview
--------

`unpkg` is a simple script to wrap the rough edges of command line archive 
programs.  It always makes sure that the unarchive results in at most 1 
directory, so you don't accidentally spew in your current dir, and by default
deletes the original archive so, like me, you don't leave them lying around.
(You can always download it again, right?)

Examples
--------

    % tar cf foo.tar a b c
    % unpkg foo.tar   # you now have a directory foo/ and no foo.tar
    % <download some files>
    % unpkg foo.zip
    % unpkg foo.tgz
    % unpkg foo.tar.gz
    % unpkg foo.rar
    % unpkg foo.7z

Usage
-----

Run `unpkg -h`
