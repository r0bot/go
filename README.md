# go
Go examples

### Async/Await
	
	//Create a channel to hold the result
	c := make(chan int, 1)
	go func() {c <- process() }() 	//async
	//Wait for the result as the function process is asynchronous
	v := <-c 						//await


### Best practices

#### Better to optimize for faster recovery (MTTR) than for avoiding failure (MTBF)


*MTTR - mean time to recovery
*MTBF - meant time between failure