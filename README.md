### Siamese_Networks

In this example we will look at Siamese Networks. These are very useful when we have things that we want to compare. A classic example is a verification problem, where we want to tell if two things are the same. In our example, we're going to try and work out if two items of clothing are the same type of thing.

### Contrastive_Loss

In this example we will continue our exploration of Siamese networks. Our first Siamese Network used binary cross entropy. This worked ok for telling us if things were the same, or different, but didn't really say how similar or how different things are. Often in machine learning, we'd like to rank things by similarity. For example, consider a biometrics scenario. We might want to find a suspect in CCTV, but rather than check if each and every person is the one we're after, it makes more sense to return the best  
  matches. However to do this, we need a way to quantify how similar things are. This is where contrastive loss comes in.

### Triplet_Loss

What's better than a pair of images? Three images! With this realisation, the triplet loss was born.

The triplet loss really just extends the siamese networks by making them bigger. Now we have three streams, three images, and a loss that looks all of those together. Cricially, the triplet is made of two image from the same class, and one from a second, different, class. So when the network evalautes a triplet of images, it evaluates a positive pair, and a negative pair simultaenously.
