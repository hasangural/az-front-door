This code shows that how you can deploy Azure Front Door Profile and Web Application Firewall policies for your web application with Azure Resource Manager Template. This template has been developed for you are already running Web App on the Azure Region. When you deploy this template, you also need to provide your web App Address or FQDN.
This template needs parameters which will be used for deployment process. 

One of the primary functions of a Reverse Proxy or WaF solution is to block traffic coming directly to the back-end service and force all incoming traffic via the security appliance. This can be achieved with AFDs Web App Firewall Settings. In order to achieve this using the IP Access Restrictions section of the Azure Web App, restrict incoming traffic to only be accepted from the AFD address space
*  **IPv4 – 147.243.0.0/16**
*  **IPv6 – 2a01:111:2050::/44**

Azure Front Door Service is a global service. So, we do not have a chance to get IP Range for Azure Front Door Instance.

Description | Link | Visualize
--- | --- | ---
Full deploy - Azure Front Door Service with Web App  | <a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fhasangural%2Faz-front-door%2Fmaster%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a> | <a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fhasangural%2Faz-front-door%2Fmaster%2Fazuredeploy.json" target="_blank"><img src="http://armviz.io/visualizebutton.png"/></a>