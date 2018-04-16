# amqp

This is a basic command line interface program that uses pika and rabbitqm in order to send messages from a host to a client.

#### Usage Notes:
* It follows the rabbitmq tutorial that can be found [here]('https://www.rabbitmq.com/tutorials/tutorial-one-python.html').
* Rabbitmq can be installed on macOS through homebrew, [instructions]('https://www.rabbitmq.com/install-homebrew.html). 
* It requires a running rabbitmq server on localhost.

#### Non-Blocking vs Blocking Operations
* Non-Blocking is when the sender does not wait for a signal to tell the sender that the reciever has processed the message.
This is different than a receipt.
* Blocking will wait for acknowledgement that a message has processed, and if not recieved it will resend the messge.