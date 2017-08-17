Recursively calculate the memory size of any thing in Go.

The private member will be ignored, because currently its not possible
to access the private member by reflection.

I will try my best to make it close to the real size, but because of the GC nature of
golang, the safety is not guaranteed. So in case you have a more precise way to calculate
the size, you can implement the `Sizable` interface of each item.