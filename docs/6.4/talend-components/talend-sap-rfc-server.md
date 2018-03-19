
# Talend SAP RFC Server

![RFC][RFCImage]

Talend SAP RFC Server is a standalone server that acts as a gateway between Talend Studio and an SAP server. It receives IDoc documents from the SAP server and makes them available for processing in Talend Jobs.

- It utilises a JMS queue to collect IDoc documents.
- Talend Data Mapper can be used to parse the IDoc’s.

### Browsing IDoc Types
![SAPRFC](./../resources/images/components/SAPRFC.png)

### Simple Job Flow

![SapJob](./../resources/images/components/SAPJob.png)

To see how to configure SAP to operate with the Talend SAP RFC Server please click [link][RFCSetup] 

<!-- links -->
[RFCSetup]: https://help.talend.com/reader/l4K8UxOw8Sq2gL_98eV_AQ/XTBZ10mfThW6CMwFrWvLdg "Artifact Repository Details"
[RFCImage]: https://help.talend.com/api/fluidtopicsclient/resources/9g5xugYWkj6RbKCiRpbI6Q/content "RFC Server Architecture"
