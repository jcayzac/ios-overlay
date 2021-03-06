#iOS SDK Overlay

##Installation

* Install [Git](http://git-scm.com/)
* git clone git://github.com/jcayzac/ios-overlay.git

##Building libraries

Example: building the [Boost C++ Libraries](http://www.boost.org/).

* Open a terminal
* Run <code>source/boost/build</code>

If all goes fine, headers should be installed in <code>/iOS_SDK_Overlay/overlay/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS?.?.sdk/usr</code>.

###Target SDK

By default, the toolchain targets the latest iOS SDK available on the host computer. You can target an older SDK, for instance *iPhoneOS4.1*, by issuing:

<code>source/boost/build SDK=4.1</code>

###Using LLVM

To be documented

##Using the overlay in an Xcode project

* Add the following in your __Header Search Paths__ setting: <code>/iOS_SDK_Overlay/overlay/$(SDK_DIR)/usr/include</code>
* Add the following in your __Library Search Paths__ setting: <code>/iOS_SDK_Overlay/overlay/$(SDK_DIR)/usr/lib</code>
* Add any library you want to link against, by name, to the __Other Linker Flags__ setting. For instance: <code>-lminizip -lbz2 -lebml</code>
* Build, run, enjoy!

##Updating the overlay

    cd /iOS_SDK_Overlay
    git pull
	...see what changed and rebuild accordingly

##License
Short version: it's BSD.

Long boring version:


    Copyright 2010 Julien Cayzac. All rights reserved.

    Redistribution and use in source and binary forms, with or without modification, are
    permitted provided that the following conditions are met:

       1. Redistributions of source code must retain the above copyright notice, this list of
          conditions and the following disclaimer.

       2. Redistributions in binary form must reproduce the above copyright notice, this list
          of conditions and the following disclaimer in the documentation and/or other materials
          provided with the distribution.

    THIS SOFTWARE IS PROVIDED BY JULIEN CAYZAC _AS IS_ AND ANY EXPRESS OR IMPLIED
    WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
    FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL JULIEN CAYZAC OR
    CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
    CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
    SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
    ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
    NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
    ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

    The views and conclusions contained in the software and documentation are those of the
    authors and should not be interpreted as representing official policies, either expressed
    or implied, of Julien Cayzac.

