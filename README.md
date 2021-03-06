# Stingray Terraform Provider [![Build Status](https://secure.travis-ci.org/whitepages/terraform-provider-stingray.png)](http://travis-ci.org/whitepages/terraform-provider-stingray)

The Stingray Terraform provider is used to interact with the Stingray
load balancer.

## Example usage

```
provider "stingray" {
	host = "https://example:9070""
	username = "username"
	password = "password"
}
```

## Argument Reference

* `host` - The protocol, host name, and port for the Stingray REST API
* `username` - The username for authenticating against the API
* `password` - The password for authenticating against the API
* `verify_ssl` - Perform SSL verification, default is true

## Supported Resources

See the `resource_*.go` files for available resources and the
supported arguments for each resource.

Support for resources is being added as needed. **Bold** resources are
fully supported.

- [x] **Action Program**
- [ ] Alerting Action
- [ ] Aptimizer Application Scope
- [ ] Aptimizer Profile
- [ ] Bandwidth Class
- [ ] Cloud Credentials
- [ ] Custom configuration set
- [ ] Event Type
- [x] **Extra File**
- [ ] GLB Service
- [ ] Global Settings
- [x] **License**
- [ ] Location
- [x] Monitor
- [x] **Monitor Program**
- [ ] NAT Configuration
- [x] Pool
- [ ] Protection Class
- [x] **Rate Shaping Class**
- [x] **Rule**
- [x] **SLM Class**
- [ ] SSL Client Key Pair
- [x] **SSL Key Pair** 
- [x] **SSL Trusted Certificate**
- [ ] Security Settings
- [ ] Session Persistence Class
- [x] Traffic IP Group
- [ ] Traffic Manager
- [ ] TrafficScript Authenticator
- [ ] User Authenticator
- [ ] User Group
- [x] Virtual Server

## Building

Dependencies are vendored (using `godep save -r`). Running `go
install` will build and install the `terraform-provider-stingray`
binary.
