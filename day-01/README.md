# Day 01 – Cloud Service Models & Shared Responsibility

## What I Learned

### Cloud Service Models
Cloud services can be grouped into three primary models:  

1. **Infrastructure as a Service (IaaS)**  
   - Provider manages: physical hardware (servers, storage, networking) and virtualization.  
   - Consumer manages: OS, middleware, runtime, applications, and data.  
   - **Use cases**: backup, disaster recovery (BC/DR), storage, archiving.  
   - **Security**: consumer has maximum control over data security but must handle OS and application patching.  
   - **Responsibility**: Infrastructure security is shared between provider and consumer.  

2. **Platform as a Service (PaaS)**  
   - Provider manages: infrastructure and operating system (including patching & updates).  
   - Consumer manages: application and data, with limited configuration responsibilities.  
   - **Use cases**: software development and testing environments.  
   - **Security**: provider ensures OS/platform security, while consumer secures application logic and data.  
   - **Responsibility**: platform security is shared.  

3. **Software as a Service (SaaS)**  
   - Provider manages: infrastructure, platform, and applications (patching, administration, updates).  
   - Consumer manages: only data and some application configurations.  
   - **Examples**: Gmail, Google Docs, Office 365.  
   - **Security**: consumer is responsible for data protection; provider ensures application and infrastructure security.  
   - **Responsibility**: application security is shared.  

---

### Shared Responsibility Model
- **Always provider responsibility**:  
  - Physical security (servers, networking, storage).  

- **Always consumer responsibility**:  
  - Data ownership, data security, governance, risk, and compliance (GRC).  

- **Shared responsibility**:  
  - **IaaS** → Infrastructure security.  
  - **PaaS** → Platform security.  
  - **SaaS** → Application security.  

The **shared areas carry the highest risk**, as both parties must establish clear separation of duties. These responsibilities should always be explicitly defined in the **Service Level Agreements (SLAs)** to avoid gaps or conflicts.  

---

## Reflection
Day-01 focused on understanding the **differences between IaaS, PaaS, and SaaS**, along with the **shared responsibility model**. The key takeaway is that responsibilities shift depending on the service model, but **data security always remains the consumer’s responsibility**, and **physical infrastructure is always the provider’s responsibility**. This foundation is critical for cloud governance and CCSP preparation.  
