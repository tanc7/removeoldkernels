https://askubuntu.com/questions/1253347/how-to-easily-remove-old-kernels-in-ubuntu-20-04-lts
Run the script as root and pipe it to a file named kernels_to_delete.txt
Edit the text file and remove all lines down to Old Kernels to be removed

Then run as root
`cat kernels_to_delete.txt | xargs sudo apt purge -y`
