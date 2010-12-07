#iOS SDK Overlay

##Installation

* Install [Git](http://git-scm.com/)
* git clone git://github.com/jcayzac/ios-overlay.git
* Add the following line to your <code>.profile</code> or <code>.bash_profile</code>:

<code>export IOS_OVERLAY_PATH="/path/to/your/ios-overlay"</code>

##Building libraries

Example: building the [Boost C++ Libraries](http://www.boost.org/).

* Open a terminal
* Run <code>${IOS_OVERLAY_PATH}/source/boost/build</code>

If all goes fine, headers should be installed in <code>${IOS_OVERLAY_PATH}/overlay/Developer/Platforms/iPhoneOS.platform/Developer/SDKs/iPhoneOS?.?.sdk/usr</code>.

###Target SDK

By default, the toolchain targets the latest iOS SDK available on the host computer. You can target an older SDK, for instance *iPhoneOS4.1*, by issuing:

<code>${IOS_OVERLAY_PATH}/source/boost/build SDK=4.1</code>

###Using LLVM

To be documented

##Using the overlay in an Xcode project

* Add the following in your *Header Search Paths* setting (curly brackets and parenthesis are important):

<code>${IOS_OVERLAY_PATH}/overlay/$(SDK_DIR)/usr/include</code>

* Add the following in your *Library Search Paths* setting (curly brackets and parenthesis are important):

<code>${IOS_OVERLAY_PATH}/overlay/$(SDK_DIR)/usr/lib</code>

* Build, run, enjoy!

