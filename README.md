# Hey there! You are using WhatsApp

This is the github repository for the extended version of the paper [Hey there! You are using WhatsApp: Enumerating Three Billion Accounts for Security and Privacy](./Hey_there_You_are_using_WhatsApp.pdf).

## Abstract 

WhatsApp, with 3.5 billion active accounts as of early 2025, is the world's largest instant messaging platform. 
Given its massive user base, WhatsApp plays a critical role in global communication.

To initiate conversations, users must first discover whether their contacts are registered on the platform.
This is achieved by querying WhatsApp's servers with mobile phone numbers extracted from the user’s address book (if they allowed access). This architecture inherently enables phone number enumeration, as the service must allow legitimate users to query contact availability. While rate limiting is a standard defense against abuse, we revisit the problem and show that WhatsApp remains highly vulnerable to enumeration at scale.
In our study, we were able to probe over a hundred million phone numbers per hour without encountering blocking or effective rate limiting.

Our findings demonstrate not only the persistence but the severity of this vulnerability.
We further show that nearly half of the phone numbers disclosed in the 2021 Facebook data leak are still active on WhatsApp, underlining the enduring risks associated with such exposures. Moreover, we were able to perform a census of WhatsApp users, providing a glimpse on the macroscopic insights a large messaging service is able to generate even though the messages themselves are end-to-end encrypted. Using the gathered data, we also discovered the re-use of certain X25519 keys across different devices and phone numbers, indicating either insecure (custom) implementations, or fraudulent activity.

In this updated version of the paper, we also provide insights into the collaborative remediation process through which we confirmed that the underlying rate-limiting issue had been resolved. 


## Cite

**Bibtex entry:**
```bibtex
@inproceedings{GFGUJ_2026,
  author       = {Gabriel K. Gegenhuber and
                  Philipp {\'E}. Frenzel and
                  Maximilian G{\"u}nther and
                  Johanna Ullrich and
                  Aljosha Judmayer},
  title        = {{Hey there! You are using WhatsApp: Enumerating Three Billion Accounts for Security and Privacy}},
  booktitle    = {{33rd Annual Network and Distributed System Security Symposium, ({NDSS}) 
                   2026, San Diego, California, USA, February 23--27, 2026}},
  publisher    = {The Internet Society},
  year         = {2026},
  url          = {https://github.com/sbaresearch/whatsapp-census},
  doi          = {https://dx.doi.org/10.14722/ndss.2026.230805},
  timestamp    = {2025-11-18T15:00:00+01:00},
}
```



