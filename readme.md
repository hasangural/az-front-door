This code shows that how you can deploy Azure Front Door Profile and Web Application Firewall policies for your web application with Azure Resource Manager Template. This template has been developed for you are already running Web App on the Azure Region. When you deploy this template, you also need to provide your web App Address or FQDN.
This template needs parameters which will be used for deployment process. 

As you may know that typical concern in a Reverse Proxy or WaF solution are to block traffic coming directly to the back-end service. That is possible to do that with Web App Firewall Settings. If you want to block traffic for direct accessing to your Web App, you should consider to add Fron Door Service IP Addresses on the'Access Restrictions' settings on the your Azure Web App
*  **IPv4 – 147.243.0.0/16**
*  **IPv6 – 2a01:111:2050::/44**

Azure Front Door Service is a global service. So, we do not have a chance to get IP Range for Azure Front Door Instance.

Description | Link | Visualize
--- | --- | ---
Full deploy - Azure Front Door Service with Web App  | <a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fhasangural%2Faz-front-door%2Fmaster%2Fazuredeploy.json" target="_blank"><img src="http://azuredeploy.net/deploybutton.png"/></a> | <a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fhasangural%2Faz-front-door%2Fmaster%2Fazuredeploy.json" target="_blank"><img src="http://armviz.io/visualizebutton.png"/></a>