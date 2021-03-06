# Hashgraph

Implementation of the use case "Game of Thrones" with Hashgraph.

There are two sdk's, one for swirlds (https://www.swirlds.com/download/) and one for hedera hashgraph (https://github.com/hashgraph/hedera-sdk-java).
Swirlds sdk provides java classes to work with the consenus algorithm called "hashgraph". Hedera hashgraph is a public network based on hashgraph. To interact with Hedera hashgraph, one needs to be a registered testnet user. As of May 2019, testnet registration was closed. Swirlds can be downloaded any time, to build a private network. Therefore we used swirlds for our use case.

To get a hashgraph demo from the swirlds sdk up and running, we followed this easy-to-understand tutorial: https://medium.com/hackers-at-cambridge/building-with-hashgraph-part-2-technical-workthrough-af63eefa53f2.

You need to have java and maven installed for compiling and running any programs via swirlds sdk. In the `config.txt` file, you have to outcomment the program you want to compile (all steps are described in the tutorial). Then cd into `source/demos/THE_PROGRAM_TO_COMPILE` and type `mvn deploy` to compile the source code to a `jar` file. Then cd back into the root of the sdk folder, and run `java -jar swirlds.jar` in the terminal. The program you chose to compile should start to run and should open 4 small and one big window on your machine.

If you want to change the code in the demos, take a look at the files `*DemoMain.java` and `*DemoState.java` inside the
`source/demos/THE_PROGRAM_TO_COMPILE/src` folder.

## Licence

This project is licensed under the MIT license. For more information see LICENSE.md.

```
The MIT License

Copyright (c) 2019 block42 Blockchain Company GmbH

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
