# VM Naming Convention

This repository provides a standardized naming convention for virtual machines (VMs) to ensure consistent and meaningful identification within the infrastructure.

## General Format
```
<Application>-<Service>-<Environment>-<Identifier>
```
## Considerations for Azure Entra ID
When configuring VM names in Azure Entra ID (formerly Azure AD), it’s important to note that the device name, including VMs, has a maximum length of 15 characters. This limitation aligns with the Windows restriction for device names. Ensuring that your VM names do not exceed this limit is crucial for maintaining compatibility and avoiding integration issues with the Entra ID domain.
## Naming Components
1. **Application (+3 characters):**
   - VCEN (VCenter Application)
   - K8S (Kubernetes)
   - ERP (Enterprise Resource Planning)
   - CRM (Customer Relationship Management)
2. **Service (3 characters):**
   - APP (Application)
   - WEB (Web Service)
   - DB (Database)
   - BCK (Backup)
   - LB (Load Balancer)

3. **Environment (4 characters):**
   - PROD (Production)
   - HMLG (Homologation)
   - DEVL (Development)

4. **Identifier (3 characters):**
   - Sequential number or unique identifier

## Service Characteristics

### APP (Application)
- **Description**: Refers to business applications or internal services with multiple functionalities.
- **Examples**:
  - Backend applications that process data.
  - Applications executing specific tasks like payment processing or inventory management.
  - Corporate applications like ERP (Enterprise Resource Planning) and CRM (Customer Relationship Management).

### WEB (Web Service)
- **Description**: Refers specifically to services that serve web content or APIs over HTTP/HTTPS.
- **Examples**:
  - Corporate websites.
  - Customer portals.
  - Public APIs providing data via HTTP/HTTPS.

### DBA (Database)
- **Description**: Refers to database services that store and manage data.
- **Examples**:
  - MySQL, PostgreSQL, Oracle databases.
  - NoSQL databases like MongoDB, Cassandra.

### BCK (Backup)
- **Description**: Refers to backup services that ensure data is replicated and recoverable in case of failure.
- **Examples**:
  - Scheduled data backups.
  - Replicated storage solutions.

### LBA (Load Balancer)
- **Description**: Refers to load balancing services that distribute network or application traffic across multiple servers.
- **Examples**:
  - HAProxy, Nginx, or other load balancing software.
  - Cloud load balancers like AWS ELB, Azure Load Balancer.

## Examples

- VCE,Application,Production, Identifier 001:
```
vce-app-prd-001
```
- Rancher, Application,Homologation, Identifier 002:
```
rch-app-hml-002
```

- ERP,Database,Development, Identifier 003:
```
erp-dba-dev-001
```


## Usage

This naming convention should be followed to ensure clarity and consistency across all VMs in the infrastructure. Adhering to this standard will facilitate management, monitoring, and support of virtual machines.

## Contributing

Please feel free to contribute to this repository by submitting issues or pull requests with suggestions or improvements to the naming convention.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
