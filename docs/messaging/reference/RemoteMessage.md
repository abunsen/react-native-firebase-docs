# RemoteMessage

```
firebase.messaging.RemoteMessage
```

### RemoteMessage
[method]new RemoteMessage();[/method]

A RemoteMessage can be sent and received through FCM.

To send a RemoteMessage, first populate it by using the `setX` methods described below, then pass it to `firebase.messaging().sendMessage(message)`;

## Properties

### collapseKey
[method]collapseKey returns nullable string;[/method]

Gets the collapse key of the message.

### data
[method]data returns Object;[/method]

Gets the message payload data.

### from
[method]from returns nullable string;[/method]

Gets the send of the message.

This will be the sender ID or the topic for topic messages.

### messageId
[method]messageId returns string;[/method]

Gets the message's ID.

This will be the message ID set when sending the message or automatically generated by the server.

### messageType
[method]messageType returns nullable string;[/method]

Gets the type of the message.

### sentTime
[method]sentTime returns nullable number;[/method]

Gets the time in milliseconds from the Epoch that the message was sent.

### to
[method]to returns string;[/method]

Get the message destination.

### ttl
[method]ttl returns number;[/method]

Gets the message time to live (TTL) in seconds.

## Methods

### setCollapseKey
[method]setCollapseKey(collapseKey) returns [ref messaging.RemoteMessage];[/method]

Sets the collapseKey for the message.

| Parameter |         |
| --------- | ------- |
| collapseKey  | **string** <br /> The collapse key. |

### setData
[method]setData(data) returns [ref messaging.RemoteMessage];[/method]

Sets the payload for the message.

| Parameter |         |
| --------- | ------- |
| payload  | **Object** <br /> The message payload. |

### setMessageId
[method]setMessageId(messageId) returns [ref messaging.RemoteMessage];[/method]

Sets the messageId for the message.

| Parameter |         |
| --------- | ------- |
| messageId  | **string** <br /> The message ID. |

### setMessageType
[method]setMessageType(messageId) returns [ref messaging.RemoteMessage];[/method]

Sets the messageId for the message.

| Parameter |         |
| --------- | ------- |
| messageId  | **string** <br /> The message ID. |

### setTo
[method]setTo(to) returns [ref messaging.RemoteMessage];[/method]

Sets the destination for the message.

| Parameter |         |
| --------- | ------- |
| to  | **string** <br /> The message destination. |

### setTtl
[method]setTtl(ttl) returns [ref messaging.RemoteMessage];[/method]

Sets the time to live (TTL) for the message.

| Parameter |         |
| --------- | ------- |
| ttl  | **number** <br /> The message time to live (TTL) in seconds. |
