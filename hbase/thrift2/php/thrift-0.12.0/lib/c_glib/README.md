Thrift C Software Library

License
=======

Licensed to the Apache Software Foundation (ASF) under one
or more contributor license agreements. See the NOTICE file
distributed with this work for additional information
regarding copyright ownership. The ASF licenses this file
to you under the Apache License, Version 2.0 (the
"License"); you may not use this file except in compliance
with the License. You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing,
software distributed under the License is distributed on an
"AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
KIND, either express or implied. See the License for the
specific language governing permissions and limitations
under the License.

Using Thrift with C
===================

The Thrift C libraries are built using the GNU tools.  Follow the instructions
in the top-level README in order to generate the Makefiles.

Dependencies
============

GLib
http://www.gtk.org/

Breaking Changes
================

0.12.0
------

The compiler's handling of namespaces when generating the name of types,
functions and header files has been improved. This means code written to use
classes generated by previous versions of the compiler may need to be updated to
reflect the proper convention for class names, which is

- A lowercase, [snake-case](https://en.wikipedia.org/wiki/Snake_case)
  representation of the class' namespace, followed by
- An underscore and
- A lowercase, snake-case representation of the class' name.