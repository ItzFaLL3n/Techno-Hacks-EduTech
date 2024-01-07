# Password Cracking through Hashcat and John the Ripper
Cracking a simple password like "password123" using tools like Hashcat and John the Ripper.

# Procedure
1.  Convert the password ("password123" in this case) to hash form. (MD5 is used in this task)
2.  Store the hash in a file.
3.  Install wordlists on kali by entering the command:

        sudo apt install wordlists

# Hashcat
->  Navigate to the location of file which contains the hash.  
->  Enter this command:

        sudo hashcat -a 0 -m 0 <name_of_file_in_which_hash_is_stored> /usr/share/wordlists/rockyou.txt

#Using A Hash Generator
#Note i'm Using a Hash Generator To Generate Password 
#i'm Not Using Hashcat(For The Tuto)

# John the Ripper
->Type:

    wordlists

->  Enter this command:

    john  --format=Raw-MD5  --wordlist=/usr/share/wordlists/rockyou.txt <location_of_file_in_which_hash_is_stored>



https://github.com/ItzFaLL3n/Techno-Hacks-EduTech/assets/94567401/87841db8-c335-40ef-8dcd-5bd0ba287d20

