# Subnet Mask Size Calculation Exercise

Using what you learned in class, answer the following questions:

### 1. What is the subnet mask for a network that can support **1000 hosts**?
Answer:  
> {(2^10) - 2} = 1024 - 2 = 1022


### 2. What is the subnet mask for a network that can support **1,000,000 hosts**?
Answer:  
> {(2^20) - 2} = 1,048.576 - 2 = 1,048.574

### 3. What is the subnet mask for a network that can support **128 hosts**?
Answer:  
> {(2^8) - 2} = 256 - 2 = 254

### 4. What is the subnet mask for a network that can support **126 hosts**?
Answer:  
> {(2^7) - 2} = 128 - 2 = 126

### 5. Why do questions 3 and 4 have different answers?

Answer:
> When we are calculating the number of host based on powers of 2,
**two addresses must be subtracted** because:

> One address is used for the **Network Identifier**

> One address is used for the **Broadcast Address**

> Therefore, if **128 host are required** and
> 2^7 = 128 This is **not enough**, because after subtracting the two
> reserved addresses, there would only be **126 usable host**.
> For that reason, the value must be increased to:
> 2^8 = 256


### 6. How many hosts can the following subnet masks support?

### Host Capacity for the Following Subnet Masks

| Subnet Mask       | Total Addresses | Usable Hosts |
|-------------------|----------------|--------------|
| 255.248.0.0       |   524,288      | 524,286      |
| 255.255.248.0     |   2048         | 2046         |
| 255.255.128.0     |   32,768       | 32,762       |
| 255.192.0.0       |   4,194.304    | 4,194.302    |
| 255.255.255.0     |   256          | 254          |