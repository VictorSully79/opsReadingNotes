# Cyber Risk Analysis

notes taken from <https://resources.infosecinstitute.com/certification/security-risk-management/>

## Risk

All aspects of life involve risk. Risk in tech has evolved just like the risk in life. The longer your around the more things you have at risk. 

CISSP Major Risk Components:

1. Information security within the organization / Security Model
2. The triad of information security – Confidentiality, Integrity and Availability
3. Security governance principles
4. Business continuity requirements
5. Policies, standards, procedures, and guidelines
6. Risk management concepts
7. Threat modeling

## Goals of a Secrity Model

1. Have contorls in place to support the mission of the organization.
2. All the decisions should be based on risk tolerance of organization, cost and benefit.

## Security Fundamentals

### Confidentiality: Prevent unauthorized disclosure

Keys:

1. Social Engineering: Training and awareness, defining Separation of Duties at the tactical level, enforcing policies and conducting Vulnerability Assessments
2. Media Reuse: Proper Sanitization Strategies
3. Eavesdropping: Use of encryption and keeping sensitive information off the network with adequate access controls

### Integrity: Detect modification of information

Keys:

1. Encryption – Integrity based algorithms
2. Intentional or Malicious Modification
   * Message Digest (Hash)
   * MAC
   * Digital Signatures

### Availability: Provide timely and reliable access to resources

Keys:

1. Prevent single point of failure
2. Comprehensive fault tolerance (Data, Hard Drives, Servers, Network Links, ets.)

## Best Practices to support CIA

1. Separation of Duties: Don't put all your eggs in one basket. Diversity of power.
2. Mandatory Vacations: Make sure other people know how to do the job by making the usual guy leave.
3. Job rotation: See Above
4. Least Privilege: See #1. Know who can do what and diversify.
5. Need to know: Just because they want to know doesn't mean they need to.
6. Dual Control: Diversify and make sure someone doesn't have a monopoly on your system.

