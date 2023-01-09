# Additional Data Repository

An Additional Data Repository is a source of Additional Data. URIs pointing to the ADR may be passed in a call, in an EIDO, or by other mechanisms. Each URI could point to a different ADR. In response to an HTTPS GET of the URI, the ADR returns the referenced Additional Data block.

An emergency call MUST have at least two  Call-Info header fields, each with a URI that resolves to an Additional Data structure (RFC 7852) \(the required block types are EmergencyCallData.ProviderInfo and EmergencyCallData.ServiceInfo). Each URI may be a Content Identifier (CID) that references an Additional Data block in the in the body of an INVITE or MESSAGE, or an HTTPS URI to an external source. Additionally, the <provided-by> element of a PIDF LO may contain an Additional Data URI or an Additional Data block. The external database that dereferences external Additional Data URIs is an Additional Data Repository (ADR). There is a minimum amount of information listed as Mandatory for EmergencyCallData.ProviderInfo and EmergencyCallData.ServiceInfo that, when combined with information from the PIDF LO and the SIP INVITE or MESSAGE, is minimally equivalent to the information currently provided by all originating networks in the ALI.

## Owner

The owner of this repository approves all changes to the repository. 

This repository is owned by the NENA Core Services Committee, i3 Architecture working group.

#### Rules:

Specification Required. 

#### Contact:

[https://www.nena.org/page/911CoreSvcs](https://www.nena.org/page/911CoreSvcs) 

## Version History

### Geocode Conversion Service v 1.0

Version 1 OpenAPI schema for this service was originally defined in NENA-STA-010.3.2021. See https://www.nena.org/page/i3_Stage
