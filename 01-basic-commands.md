SSH key related commands 
To generate SSH key from your system 

'''
ssh-keygen -f <file-name-to-key>
'''
To login to any linux server using Public-key and Private-key for this, before creating server you need to put your public-key in server by import key-pair option in AWS

'''
ssh -i <private-key> user-name@ip address
'''

