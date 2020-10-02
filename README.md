# DeployingWebsites

1. Navigate https://portal.azure.com/#create/Microsoft.SQLDatabase and create a new database - Ensure you have the correct datasize configuration and subscriptions.
2. Add client Ip address to the firewall settings
3. Navigate to overview to see server Name - Ensure you can connect with Sql Server Managment Studio
4. Create a new Asp.net Standard Web API Application 4.7.2
5. Ensure you are able to run the application and that it is pointing to the right local server (iisExpress/ local IIS)
6. Update the Boostrap Version
7. After deploy edit web.config file and remove all code in system.codedom  
8. add <system.web>
   <trust level="Full"/>
</system.web>
9. Settings : delete existing files,  precompile and exclude files from the app_data in advanced configure settings uncheck allow precompile and emit debug
