#md5sum this command checks a file’s MD5 hash to verify if the file has been changed.
#sha256sum creates a SHA-256 hash that can be used to check a file’s integrity.
#gpg --gen-key the gpg stands for GNU privacy guard key pair, it is used to create a new GPG key pair(public and private keys).
#gpg --encrypt encrypts a file so that only the intended person can access it.
#gpg --decrypt decrypts an encrypted file back into its original readable form.
#chattr +i  makes a file immutable, this means if this command is run on a file, it cannot be edited, modified, deleted,renamed or anything of such, unless if a chattr -i is run on the file.
#lsattr this command shows the special attributes set on a file,usually to see files that chattr +i command was run on.
#ufw enable ufw stands for uncomplicated firewall it turns on the firewall to start protecting the system.
#ufw allow this sllows specific network traffic or ports through the firewall.
#ufw status shows whether the firewall is active and the rules that are currently set.