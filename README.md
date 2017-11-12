# BluetoothTesting

####Connected/Connecting Bluetooth socket
1. SERVER SIDE
- Use BluetoothServerSocket for listening
- When connection accepted, returns new BluetootSocket for managing
- ??How do you know if it's accepted??
2. CLIENT SIDE
- Use single BluetoothSocket for outgoing connection + managing
3. BTSocket = RFCOMM/SPP

####Creating BluetoothSocket
1. For known devices, use: BluetoothDevice.createRfcommSocketToServiceRecord()
2. Call .connect() to connect to remote to block until connection established or fails
3. Same as BTServerSocket
