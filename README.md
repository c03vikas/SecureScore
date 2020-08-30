# SecureScore
Azure Security Score ARM 

1. This deployment will create a Logic App which will pull the data on daily basis & store into Custom table under Log Analytics workspace. 

2. Resources created will be Logic App, Azure Monitor Workbook, Log Analytics workspace & API Connection. It is recommended to create a new Resource Group for the se resources. 

3. Once deployment of this ARM template is complete please go to all the Suscriptions & provide this Logic App as Reader RABC role.

4. Make sure all selected subscriptions registered to Azure Security Center.


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fc03vikas%2FSecureScore%2Fmaster%2FSecureScoreARM.json" target="_blank">
  <img src="https://aka.ms/deploytoazurebutton"/>
</a>


5. Please note that First time you'll need to manually trigger the Logic App.

6. Once Logic App is executed it will create Four Custom new tables in Log Analytics workspace: SecureScore_CL, SecureScoreAssessments_CL, SecureScoreControls_CL and Subscriptions_CL.

 
