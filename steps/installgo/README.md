Create and navigate to a directory for the latest release of Go to be 
downloaded.

Navigate to the [official Go downloads page](https://go.dev/dl/) in your 
web browser. From there, copy the URL for the current binary release's 
tarball.

Use the `curl` command to retriece the tarball file. The `-O` flag ensures 
that this outputs to a file, and the `-L` flag instructs HTTPS redirects.

To verify the integrity of the file you downloaded, run the `sha256sum` 
command and pass it the filename as an argument. The checksum should match 
the one listed on the website.

Use `tar` to extract the tarball file. The `-C` flag instructs tar to change 
to given directory before performing any operations. The `-x` flag tells `tar` 
to extract, `-v` tells tar to be verbose, and `-f` tells `tar` the file.

Finally, cleanup the downloaded files.