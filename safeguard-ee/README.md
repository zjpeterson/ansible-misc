# safeguard-ee

This is an Execution Environment spec that supplies access to the `oneidentity.safeguard` collection found at: https://github.com/OneIdentity/safeguard-ansible/tree/main/collection/oneidentity/safeguard

If you are using AAP, you should avoid using the Credential Type guidance found in that repo and only use the collection, which contains a lookup plugin. You should instead make a Custom Credential Type using the regular framework, following the documentation at: https://docs.ansible.com/automation-controller/latest/html/userguide/credential_types.html
