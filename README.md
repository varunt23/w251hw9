# w251hw9
Homework 9



For the single worker the  training the time was for one epoch 
I have uploaded the weights and biases report for this as well in the repo

For the parralel training I have created the notebook to run both workers but 
I was facing some issues with the code hanging at the line 

"model = torch.nn.parallel.DistributedDataParallel(model, device_ids=[GPU])"

even though it passed the init command. I think this may be becuase I need to set the NCCL_SOCKET_IFNAME to correct value (ens5) in the .nccl.conf file. I was unable to figure this part out and thus was unfortunately unable to run the parralel workers. As a result I was unable to calculate the time (which should've been around half of the time for the single worker) and look at the tensorboard or weights and biases report for this.
