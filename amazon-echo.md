# Amazon Echo
The Amazon Echo is a smart speaker, that is easy to program new capabilities (skills) for. You can create skills with the official node.js SDK or you can use an unofficial .net port (which still works quite good). It is really easy to make your first skill if you have built any web API before, you can even test your skill in a web browser you dont need a physical device. 

## Prerequsites
* An Amazon developer Account

You can download this little project I created to see a sample app written in .NET 
https://github.com/sjkp/alexa.whereareyou it uses this nuget: https://github.com/AreYouFreeBusy/AlexaSkillsKit.NET 

You can host your skills in Azure Web App or use Ngrok.io for local testing. 

## Project Idea
### Ask Time Registration 
Build an Alexa skill that allows people to ask questions about time reg, e.g. register hours or view how many hours they have registered

Note you might have to turn to LUIS or some other NLP service. 

## Links
(Make an alexa skill that can sign in to Azure)[https://blogs.msdn.microsoft.com/premier_developer/2016/12/12/amazon-alexa-skills-development-with-azure-active-directory-and-asp-net-core-1-0-web-api/]
(Make Alexa use LUIS)[http://www.garypretty.co.uk/2016/10/31/making-amazon-alexa-smarter-with-microsoft-cognitive-services/]
