# Federated Learning using Blockchain
An Application to demonstrate Federated Learning using Blockchain

## Federated Learning
[https://ai.googleblog.com/2017/04/federated-learning-collaborative.html](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html)
<img src="https://i.imgur.com/ljIu7Pi.png"/>

Federated Learning is simply the decentralized form of Machine Learning. In Machine Learning, we usually train our data that is aggregated from several edge devices like 
mobile phones, laptops, etc. and is brought together to a centralized server. Machine Learning algorithms, then grab this data and trains itself and finally predicts results 
for new data generated. Great!

But, can you smell a “privacy nightmare”?

The AI market is dominated by tech giants such as Google, Amazon and Microsoft, offering cloud-based AI solutions and APIs. In the traditional AI methods, sensitive user data
are sent to the servers where models are trained. That’s awful! With the increased awareness of user privacy across different devices and platforms, AI developers should not 
ignore the fact that their model is accessing and using data that is user-sensitive!

Well, here comes our Savior! The Federated Learning approach.

1. So, our centralized machine learning application will have a local copy on all devices, where users can use them according to our need.
2. The model will now gradually learn and train itself on the information inputted by the user and become smarter, time to time.
3. The devices are then allowed to transfer the training results, from the local copy of the machine learning app, back to the central server. Remember, only results, not data!
4. This same process happens across several devices, that have a local copy of the application. The results will be aggregated together in the centralized server, this time 
without user data.
5. The centralized cloud server now updates its central machine learning model from the aggregated training results, which is now far better than the previously deployed 
version.
6. The development team now updates the model to a newer version, and users update the application with the smarter model, created from their own data!

## System Architecture
<img src="https://i.postimg.cc/MpFVHzv8/arch.jpg"/>


## Distributed Linear Regression Model

> ***Directory:*** Federated (linear Regression)
>
> ***Install Python Libraries*** 
>  - numpy
>  - pandas
>  - pygad
>  - pickle
>
> ***Code Execution*** - Open 3 terminals
> - First terminal ```python server.py```
> - Second terminal ```python client1.py```
> - Third terminal ```python client2.py```

## Distributed Blockchain Model

> ***Directory:*** Federated(linear regression + blockchain) 
>
> ***Block Structure***
>> Block -
>> -    index
>> -    client_model
>> -    server_model
>> -    cli - [“cli1”, “cli2”]
>> -    timestamp
>> -    previous_hash
>> -    nonce
>
> ***Block Hashing***
>> Hash -
>>  -   index
>>  -   client_weights
>>  -   client_biases
>>  -   cli
>>  -   timestamp
>>  -   previous_hash
>>  -   nonce
> 
> ***Code Execution*** - Open 3 terminals
> - First terminal ```python server.py```
> - Second terminal ```python client1.py```
> - Third terminal ```python client2.py```
