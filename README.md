# SerialPort-APC220-C-
send and receive data by APC220 SerialPort

This Project and code has written by manash Kumar Mandal (https://github.com/manashmndl)
Because i find a bug and important variables that didn't initialized , i fix it (i spend a lot of time till i understand what's the problem and what's the bug )

At first, sometimes Arduino received unknown and bullshit characters
And then i understand some variable not inialized
I didn't do anything else and all of code wrote by him
i just initiale the variables

## Be careful !!!

in "SerialPort.cpp" and "readSerialPort function" , if you set "toRead =  0" then it try to receive character from source and if it doesn't receive anything, it will pass it and return 0
but if you set "toRead =  1" , it will stay till it receive at least one char from source
