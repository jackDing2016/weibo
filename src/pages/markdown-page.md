
# User Variables (Edit These!)


proxy="127.0.0.1:7890"


# Environement Variables
# (npm does use these variables, and they are vital to lots of applications)

 export HTTPS_PROXY="http://$proxy"

 export HTTP_PROXY="http://$proxy"

 export http_proxy="http://$proxy"

 export https_proxy="http://$proxy"

 export all_proxy="http://$proxy"

 export ftp_proxy="http://$proxy"

 export dns_proxy="http://$proxy"

 export rsync_proxy="http://$proxy"

 export no_proxy="127.0.0.10/8, localhost, 10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16"

# npm Settings

 npm config set registry http://registry.npmjs.org/

 npm config set proxy "http://$proxy"

 npm config set https-proxy "http://$proxy"

 npm config set strict-ssl false

 echo "registry=http://registry.npmjs.org/" > ~/.npmrc

 echo "proxy=http://$proxy" >> ~/.npmrc

 echo "strict-ssl=false" >> ~/.npmrc

 echo "http-proxy=http://$proxy" >> ~/.npmrc

 echo "http_proxy=http://$proxy" >> ~/.npmrc

 echo "https_proxy=http://$proxy" >> ~/.npmrc

 echo "https-proxy=http://$proxy" >> ~/.npmrc


# WGET SETTINGS
# (Bonus Settings! Not required for npm to work, but needed for lots of other programs)

 echo "https_proxy = http://$proxy/" > ~/.wgetrc

 echo "http_proxy = http://$proxy/" >> ~/.wgetrc

 echo "ftp_proxy = http://$proxy/" >> ~/.wgetrc

 echo "use_proxy = on" >> ~/.wgetrc


# CURL SETTINGS

 echo "proxy=http://$proxy" > ~/.curlrc

