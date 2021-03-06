Index of examples and theirs purpose
====================================

**dns_test.py**: Test the DNS engine of Pystack by resolving www.google.fr

**EchoServer**: An example of an EchoServer programmed using Pystack (and twisted reactor)

**hijacker.py**: Replace the socket module in sys.modules to force the usage of pystack. Then load test_client.py which is a genuine script using socket and run it.

**simple_socket.py**: Is a very tiny implementation of the module socket but using pystack

**sshserver.py**: Implementation of an SSH server over pystack (with the help of twisted)

**test.py**: Basic example of hand-crafted stack

**test_client.py**: Classic python client that use the standard module socket (hijacker.py load this file to force it to use pystack)

**webserver.py**: Implementation of a HTTP server using pystack

**hiddensite/**: Content used by the stegano website example

**mitm/**:

* mitm.py: Main of the program. Create the Qt Window and instanciate the stack.

* mitm_tcpsession.py: Implementation of the modified TCPSession to make it able to handle packet coming from nfqueue..

* tcpmodif.py: Slightly modified TCPProtocol to pull up all the connections sniffed to the Qt Window.

* window.py: Qt window code generated by QtDesigner.

**pystack_socket_test/***: Implementation of both TCP/UDP client/server, to test pystack.

**sitetest**: Pages browsed by the HTTP server implementation.

**stegano**:

* basic_steganoclient.py: Basic stegano client that use TCP headers as carrier.

* basic_steganoserver.py: Basic stegano server that also TCP headers according to the same protocol than the client.

* chat_gui.py: Code generated by QtDesigner for the chat window.

* clientweb.py: Browser window. Generated by QtDesigner.

* max_throughput_steganoserver.py: Steganographic server implementation that use the maximum of available fields to maximise throughput.

* stealth_steganoclient/server.py: Client/server that use to least possible fields to be entirely undetectable.

* stegano_chat.py: Implementation of a chat that use steganographic channels

* stegano_http_client/server.py: Implementation of an hidden HTTP server into another. (HTTP imbrication)