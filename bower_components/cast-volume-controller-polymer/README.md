Copyright 2014 Google Inc. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

#cast-volume-controller
This element represents the volume bars in the [CastVideos-chrome-material](https://github.com/googlecast/CastVideos-chrome-material) sample.  

It's used in both `cast-player-bar` and `cast-controller-element` as the volume controller.  
It fires an event to [`cast-manager`](https://github.com/googlecast/cast-manager-polymer) when volume is changed and its rendering is bound to the `volume` property.


##Setup
Use [Bower](http://bower.io/) to include the cast-volume-controller in your web app.  The following 
command will add the cast-volume-controller and it's dependencies to your project.

    bower install --save googlecast/cast-volume-controller-polymer
    
##Integration
You'll need to first include 
[Polymer](https://www.polymer-project.org/).

###Including the element
In your html include the element

    <link rel="import"
        href="bower_components/cast-volume-controller-polymer/cast-volume-controller.html">
        
Add the element to your HTML and bid the `volume` parameter.
 
    <cast-volume-controller volume="[[ volume ]]"></cast-volume-controller>
