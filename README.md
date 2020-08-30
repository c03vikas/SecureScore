# SecureScore
Azure Security Score ARM 

This deployment will create a Logic App which will pull the data on daily basis & store into Custom table under Log Analytics workspace. 

Resources created will be Logic App, Azure Monitor Workbook, Log Analytics workspace & API Connection. It is recommended to create a new Resource Group for the se resources. 

Once deployment of this ARM template is complete please go to all the Suscriptions & provide this Logic App as Reader RABC role.

Make sure all selected subscriptions registered to Azure Security Center.


<a href="https://azuredeploy.net/
   repository=https://github.com/c03vikas/SecureScore/blob/master/SecureScoreARM.json"
   target="_blank">
   <img src="https://aka.ms/deploytoazurebutton"/>
</a>


Please note that First time you'll need to manually trigger the Logic App.

Once Logic App is executed it will create Four Custom new tables in Log Analytics workspace: SecureScore_CL, SecureScoreAssessments_CL, SecureScoreControls_CL and Subscriptions_CL.

 
