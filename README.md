## Records

RTC communication procedure:

1. In `sender.html` exxcute `JSON.stringify(localConnection.localDescription.toJSON())` in console to get Local Description `LocalDescription_A`.

2. In `receiver.html` execute `setRemoteDescription($LocalDescription_A)` in console.

3. Execute `createAnswer()` in `receiver.html`

4. Obtain Local Description of b `$LocalDescription_B` by executing `JSON.stringify(localConnection.localDescription)` `receiver.html` in `receiver.html`

5. Execute `setRemoteDescription('$LocalDescription_A')` in `sender.html`

6. Bi-com start. Execute `sendChannel.send('123')` in `sender.html`.

7. Recevier html receive `event.data 123`


## Ref

https://eller.top/posts/85#%E6%B5%8B%E8%AF%95%E8%BF%9E%E6%8E%A5