# miniseed2dmc - send miniSEED to a Data Management Center

This program transfers selected miniSEED data records from the local
computer to a remote Data Management Center.  Prior to using this program
coordination with the DMC is required.

To track the miniSEED data transferred the program writes SYNC files
representing the data coverage.  Additionally, a state file is maintained
to track the progress of data transfer.  This tracking means that the client
can be shut down and then resume the transfer when the client is restarted.
More importantly it allows the client to determine when all records from
a given data set have been transferred preventing them from being transferred
again erroneously.

For usage information see the [miniseed2dmc manual](doc/miniseed2dmc.md) in the
'doc' directory.

## Building

In most Unix/Linux environments a simple 'make' will build the program.

The `CC` and `CFLAGS` environment variables can be used to configure
the build parameters.

## License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

[http://www.apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

Copyright (C) 2024 Chad Trabant, EarthScope Data Services