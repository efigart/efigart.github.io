---
layout: essay
type: essay
title: "Asking Smart Questions"
# All dates must be YYYY-MM-DD format!
date: 2025-01-30
published: false
labels:
  - Questions
  - Answers
  - StackOverflow
---

## Importance

Communication is a fundamental skill, especially in software development. Being able to ask the right questions is imperative when seeking help from peers or the open source community. The essay How to Ask Questions the Smart Way by Eric Raymond goes into detail about effective questioning. One of the main takeaways is asking yourself if asking a question is really necessary. There are many resources that are easily available to consult, a prominent example is ChatGPT or even a simple google search. These are likely to solve and maybe even expand on the problem you are facing. If those do not solve your problems, Raymond provides guidelines on how to ask an effective question. He recommends avoiding posting your question on an irrelevant forum, or asking too simple of a question. Doing so will increase the chance of you receiving a helpful response. 

## Smart 

Here is an example of a smart way to ask a question. 

[Why is processing a sorted array faster than processing an unsorted array](https://stackoverflow.com/questions/11227809/why-is-processing-a-sorted-array-faster-than-processing-an-unsorted-array).

```cpp
#include <algorithm>
#include <ctime>
#include <iostream>

int main()
{
    // Generate data
    const unsigned arraySize = 32768;
    int data[arraySize];

    for (unsigned c = 0; c < arraySize; ++c)
        data[c] = std::rand() % 256;

    // !!! With this, the next loop runs faster.
    std::sort(data, data + arraySize);

    // Test
    clock_t start = clock();
    long long sum = 0;
    for (unsigned i = 0; i < 100000; ++i)
    {
        for (unsigned c = 0; c < arraySize; ++c)
        {   // Primary loop.
            if (data[c] >= 128)
                sum += data[c];
        }
    }

    double elapsedTime = static_cast<double>(clock()-start) / CLOCKS_PER_SEC;

    std::cout << elapsedTime << '\n';
    std::cout << "sum = " << sum << '\n';
}
```

The provided code is written in C++. It genertaes a random array of random inetegrs and sorts them by value. The program then records and prints the elapsed time. Sorting the array before hand results in a run time of 1.93 seconds, without it it runs in 11.54 seconds. The user also recreated the code in Java, btu recieved a simialr result. I think this is a solid question. It is clear and straightforward, and is a relavent topic in software developemnt. Additionally, the user also provided multiple sources of code to further illustrate his point. As a result, they recived many response and were given insight into their problem. 

## Not Smart 

In order to illustrate a not-smart qustion, i utilized ChatGPT

Why doesn't my code work?

```cpp
int main() {
    int x = 10;
    int y = x * 2;
}
```

This question lacks specificity, shows very litte effort, and has very little contex of the code or what the objective is. It is not a smart question. 

## Conclusion

To conclude, being able to create smart questons is an essential skill for eductaion and the workforce. By follwing the principles written by Raymond, you will be able to communicate effectively and recive meaningful answers to any inquiry. 
