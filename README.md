# Basic Setup

1. Upgrade g++ to g++-5 as our repository uses c++14 <br/>
   Steps to upgrade here : http://askubuntu.com/questions/618474/how-to-install-the-latest-gcurrently-5-1-in-ubuntucurrently-14-04
   Verify if the upgradation is successful or not

2. Install AWS CPP SDK <br/>
   Pre-requisites : Needed CMake <br/>
   https://github.com/aws/aws-sdk-cpp <br/>
   https://aws.amazon.com/documentation/sdk-for-cpp/ <br/>
   Instructions to Install : http://sdk.amazonaws.com/cpp/api/LATEST/index.html <br/>

3. Make a git clone of our repository 
4. Run ./autogen.sh
5. Run configure
6. Run "make all" to verify build succeeds



