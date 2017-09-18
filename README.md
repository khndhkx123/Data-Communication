# Data-Communication
UDP Server &amp; Client


## Project 1: UDP Echo

### 목적: 
UDP Socket을 이용하여 메시지를 주고 받으며 화면을 통해 서로간에 통신이 가능한 기능 구현

### 내용: 
클라이언트에서는 UDP Socket을 이용하여 화면에서 keyboard를 입력 받아 서버에게 UDP 패킷를 보내고 서버로부터 온 UDP 패킷을 화면에 표시하고, 서버에서는 클라이언트에서 보낸 UDP 패킷을 그대로 다시 클라이언트로 전달하는 프로그램 구현
클라이언트에서는 Keyboard의 내용을 입력 받아 UDP 패킷을 만들고 만들어진 UDP 패킷을 IP 주소와 UDP port 번호로 정의된 상대방에게 보냄

서버에서는 받은 UDP 패킷을 그대로 송신한 클라이언트에게 돌려보냄
### Client
SendThread: 사용자가 입력한 채팅 메시지를 UDP 패킷으로 만들어 전송하는 기능
RcvThread: UDP 패킷이 오면 오는 즉시 패킷을 받고 화면에 표시해주는 기능

### Server
SendThread: 수신한 채팅 메시지를 UDP 패킷으로 만들어 송신한 Client에게 전송하는 기능
RcvThread: UDP 패킷이 오면 오는 즉시 패킷을 받고 송신한 Client를 확인하는 기능

### 할일(Mission): 
Multi Thread 기반 UDP 프로그램 완성
(Option) Timeout 기능 구현

## Project 2: Chatting Program

### 목적: 
UDP Socket을 이용하여 메시지를 주고 받으며 화면을 통해 서로간에 통신이 가능한 기능 구현

### 내용: 
UDP Socket을 이용하여 화면에서 keyboard를 입력 받아 상대에게 UDP 패킷를 보내고 상대로부터 온 UDP 패킷을 화면에 표시하면서 UDP를 통해 메시지를 주고 받는 과제 (각자 Client와 서버를 모두 포함하고 있음)
Keyboard의 내용을 입력 받아 UDP 패킷을 만들고 만들어진 UDP 패킷을 IP 주소와 UDP port 번호로 정의된 상대방에게 보냄
RcvThread: UDP 패킷이 오면 오는 즉시 패킷을 받고 화면에 표시해주는 기능

### 할일(Mission): 
Multi Thread 기반 UDP Chatting 프로그램 완성
Stop & Wait  유사한 기능 구현 (ACK & Timeout)


