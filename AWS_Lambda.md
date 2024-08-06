## AWS Lambda

In Lambda, concurrency is the number of in-flight requests that your function is currently handling. There are two types of concurrency controls available:

---
**Reserved concurrency** – This represents the maximum number of concurrent instances allocated to your function. When a function has reserved concurrency, no other function can use that concurrency. Reserved concurrency is useful for ensuring that your most critical functions always have enough concurrency to handle incoming requests. Configuring reserved concurrency for a function incurs no additional charges.

**Provisioned concurrency** – This is the number of pre-initialized execution environments allocated to your function. These execution environments are ready to respond immediately to incoming function requests. Provisioned concurrency is useful for reducing cold start latencies for functions. Configuring provisioned concurrency incurs additional charges to your AWS account.

But better visit official doc [here](https://docs.aws.amazon.com/lambda/latest/dg/configuration-concurrency.html) and [here](https://docs.aws.amazon.com/lambda/latest/dg/lambda-concurrency.html#reserved-and-provisioned)

![img.png](screenshots/img_19.png)

--- 
### Synchronous vs. Asynchronous Invocation