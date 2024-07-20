# VM Naming Convention

This repository provides a standardized naming convention for virtual machines (VMs) to ensure consistent and meaningful identification within the infrastructure.

## General Format
```
<Location>-<Environment>-<Service>-<Application>-<Identifier>
```

## Naming Components

1. **Location (3 characters):**
   - BSB (Brasília)
   - SAO (São Paulo)
   - RIO (Rio de Janeiro)

2. **Environment (4 characters):**
   - PROD (Production)
   - HMLG (Homologation)
   - DEVL (Development)

3. **Service (3 characters):**
   - APP (Application)
   - WEB (Web Service)
   - DB (Database)
   - BCK (Backup)
   - LB (Load Balancer)

4. **Application (3 characters):**
   - VCE (VCenter Application)
   - K8S (Kubernetes)
   - ERP (Enterprise Resource Planning)
   - CRM (Customer Relationship Management)

5. **Identifier (3 characters):**
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

### DB (Database)
- **Description**: Refers to database services that store and manage data.
- **Examples**:
  - MySQL, PostgreSQL, Oracle databases.
  - NoSQL databases like MongoDB, Cassandra.

### BCK (Backup)
- **Description**: Refers to backup services that ensure data is replicated and recoverable in case of failure.
- **Examples**:
  - Scheduled data backups.
  - Replicated storage solutions.

### LB (Load Balancer)
- **Description**: Refers to load balancing services that distribute network or application traffic across multiple servers.
- **Examples**:
  - HAProxy, Nginx, or other load balancing software.
  - Cloud load balancers like AWS ELB, Azure Load Balancer.

## Examples

- Brasília, Production, Application, VCE, Identifier 001:
```
BSB-PROD-APP-VCE-001
```
- Rio de Janeiro, Development, Database, ERP, Identifier 003:
```
RIO-DEVL-DB-ERP-003
```

- Brasília, Production, Backup, CRM, Identifier 004:
```
BSB-PROD-BCK-CRM-004
```


## Usage

This naming convention should be followed to ensure clarity and consistency across all VMs in the infrastructure. Adhering to this standard will facilitate management, monitoring, and support of virtual machines.

## Contributing

Please feel free to contribute to this repository by submitting issues or pull requests with suggestions or improvements to the naming convention.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
