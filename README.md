wget https://github.com/rc452860/vnet/releases/download/v0.0.6/vnet_linux_amd64 -O vnet &&chmod +x vnet

./vnet

nohup ./vnet>vnet.log 2>&1 &

kill -9 $(ps aux | grep '[v]net' | awk '{print $2}')
