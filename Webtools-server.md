# Webtools-server

## socket.io

서버-클라이언트간 이벤트 기반 통신

### 서버사이드
```
io.sockets.on('connection',socket()=>{
    
    // 클라이언트 측에서 newUser이라는 socket emit이 발생시 호출
    socket.on('newUser', (name)=>{
        socket.sam = 'bear' // 소켓 프로그래밍 전체에서 전역변수를 만들어 활용가능하다
        io.sockets.emit('update',{type:'connect',name:'SERVER', message:name+'님이 접속하였습니다.}) // type:connect이므로 connect establishment으로 보임
        // 서버사이드의 io.sockets.emit은 클라이언트 소켓함수를 부른다.
    })

    socket.on('message', (data)=>{
        console.log(data)
        socket.broadcast.emit('update',data) // 자기 자신을 제외한 모든 소켓에 뿌린다
    })

    socket.on('disconnect',()=>{
        console.log(socket.name+ ' 님이 나가셨습니다')
    })

})
```


### 클라이언트

```
var socket = io()
// connection
socket.on('connect', function(){
    if(!name) name="sam"
    socket.emit('newUser',name)
})
socket.on('update',function(data){
    console.log(data)
})
function send(){
    var message = document.getElementById('test').value
    document.getElementById('test').value =''
    socket.emit('message',{type:'message',message:message})
}
```


