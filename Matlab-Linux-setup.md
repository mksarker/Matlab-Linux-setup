# Matlab-Linux-setup

MATLAB R2015a (8.5.0.197613), 64-bit (glnx64) February 12, 2015

Installation
-----------
0. Unpack ISO:

bunzip2 R2015a-glnxa64.iso.bz2 


1. Mount ISO


sudo mkdir /media/mnt_iso

sudo mount -o loop /media/mostafa/MKSARKER/SOFTWARE/MATLAB/Mathworks_Matlab_R2015a_Linux/R2015a-glnxa64.iso /media/mnt_iso

sudo umount /media/iso


2. Copy files to some temporary directory, e.g. /tmp/matlab.


3. Replace install jar


cp fixr2015arel/install.jar /tmp/matlab/java/jar


4. In /tmp/matlab, run ./install (Not working) using below methods;


##########

sudo su

chmod 777 -R /home/yourUSER/pathTO/matlabFOLDER

cd /home/yourUSER/pathTO/matlabFOLDER

./install

############


5. Check 'Use a File Installation Key' and press Next.


6. Provide File Installation Key: 58691-35070-25550-28046-23042    //54422-40402-23817-20808-30933


7. Install


8. In your target installation directory replace libmwservices.so.

cp /media/mostafa/Data/Soft/Mathworks_Matlab_R2015a_Linux/fixr2015arel/libmwservices.so /usr/local/MATLAB/R2015a/bin/glnxa64


9. Run MATLAB /usr/local/MATLAB/R2015a/bin/matlab and select

   'Activate manually without the Internet.'.
   

10. Use license fixr2015arel/Standalone License.lic


#########################################

RUN----------------

/usr/local/MATLAB/MATLAB_Production_Server/R2015a/bin/matlab

