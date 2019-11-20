# go
Go examples

### Async/Await
	
	//Create a channel to hold the result
	c := make(chan int, 1)
	go func() {c <- process() }() 	//async
	//Wait for the result as the function process is asynchronous
	v := <-c 						//await
