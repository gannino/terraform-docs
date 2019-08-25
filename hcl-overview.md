# HCL Overview

HCL has two current variants.  [HCL](https://github.com/hashicorp/hcl) and [HCL2](https://github.com/hashicorp/hcl2). HCL2 is being merged into terraform - [#115](https://github.com/hashicorp/hcl2/issues/115), but the home repo has the core language that can be extended. 

### HCL Docs 
HCL (HashiCorp Configuration Language) is a configuration language built by HashiCorp. The goal of HCL is to build a structured configuration language that is both human and machine friendly for use with command-line tools, but specifically targeted towards DevOps tools, servers, etc.

HCL is also fully JSON compatible. That is, JSON can be used as completely
valid input to a system expecting HCL. This helps makes systems
interoperable with other systems.

HCL is heavily inspired by
[libucl](https://github.com/vstakhov/libucl), nginx configuration, and others similar.

- [Source](https://github.com/hashicorp/hcl)

### HCL2 Docs 

Same as above basically plus:

It includes an expression syntax that allows basic inline computation and, with support from the calling application, use of variables and functions for more dynamic configuration languages.

HCL provides a set of constructs that can be used by a calling application to construct a configuration language. The application defines which attribute names and nested block types are expected, and HCL parses the configuration file, verifies that it conforms to the expected structure, and returns high-level objects that the application can use for further processing.


### HCL vs HCL2 

- HCL2 relies on a [spec file](https://github.com/hashicorp/hcl2/blob/master/cmd/hcldec/examples/npm-package/spec.hcldec) to interpret variables where as HCL can just be interpretted natively. 
    - This means that we can 

- First class support for variables
    - HCL you had to escape them with "${...}", now you don't. 