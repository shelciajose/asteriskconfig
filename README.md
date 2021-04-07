# asterisk configuration 
sudo apt-get update

sudo apt-get install bison wget openssl libssl-dev libasound2-dev libc6-dev libxml2-dev libsqlite3-dev libnewt-dev libncurses5-dev zlib1g-dev gcc g++ make perl uuid-dev git subversion libjansson-dev unixodbc-dev unixodbc-bin unixodbc autoconf libedit-dev 

cd /usr/src    
                    
sudo wget http://downloads.asterisk.org/pub/telephony/asterisk/asterisk-18-current.tar.gz 
          
sudo tar -xzvf asterisk-18-current.tar.gz                 

cd asterisk-18.3.0
            
sudo ./configure
           
sudo make 
                       
sudo make install   
        
sudo make config   
             
sudo make samples               

sudo asterisk -r
