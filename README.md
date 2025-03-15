java c
EIE1005 Fundamental AI and Data Analytics 
Workshop 3: Creating Chatbot using DialogFlow
A. Objectives and Outcomes 
After finishing this lab, you should be   able to
•          understand   the   practical   aspects   of   conversational   AI
•          know   the   basic   components   in   DialogFlow
•          master   the   fundamental   process   of   constructing   chatbots   using   DialogFlow
B. Assessment Criteria 
•          Ability   to   design   and   build   chatbots   using   DialogFlow
•          Ability   to   produce   a   working   chatbot
•          Ability to create a chatbot that is slightly different from the example shown in the lab   procedure
•            Clarity   of   the   report
C. Submission 
• In-class demonstration 
•          Capture   the   screen   and   put   the   pictures   in   your   report.
• Convert your report to PDF.
•          Submit the PDF file to Blackboard before the deadline   specified   in   Blackboard.
D. Getting Start 
1.          We   will   use   Google   DialogFlow.   You   need   a   Google   account   to   use   DialogFlow.   If you   do   not   have   a   Google   account, visit https://support.google.com/mail/answer/56256?hl=ento   create   one.   You may access DialogFlow through any browser, and no installation is required. It   is   free!
2. Sign in DialogFlow   by   visitinghttps://dialogflow.cloud.google.com/ 
3.          To   start   with   a   new   Chatbot,   you   need   to   create   an   agent.   Click   “Create   Agent”   on   the   left   panel.
Give   a name to the agent   (e.g., BikeShop)   and   click   “Create”. You   should   see   something   like   the   following.
4. Enable text-to-speech by   clicking   the   setting   symbol  on   the   left   panel.   Select   the   “Speech”
tab and “Enable Automatic Text-to-Speech”. Then, click “Save”   .
5. Customize the Default Welcome Intent:
a.         Click on the Default   Welcome Intent
b.       Navigate   to   the   Responses   section
c.         In the Text or   SSML response table, delete   all the default responses.
d.       In   the Text or SSML   response table, copy and   paste   the following   response:   “Welcome.
I can tell you about the shop   hours, or   I   can set   up   an   appointment.   Which   would you   like?”

e.         Click the “Save” button
f.          Test   your   Welcome   Intent   by   putting   “   Hi”   in   the   “Try    it   now”   edit   box   on   the   right   panel.

6. Customize the Default Fallback Intent.
a.         Click on the Default Fallback Intent.
b.       Navigate   to   the   Responses   section.
c.         In the Text or   SSML response table, delete   all the default responses.
d.       In the Text or SSML response table, copy and paste the following response: “Sorry, did   you want to   hear our   hours, or set   up an   appointment?”
e.         Click ”Save”
f.          Try something irrelevant on the   “Try   it now”   edit   box   on   the right.

7. Add some more welcome messages to   the   “Text   or   SSML   Response”   entry.   Your   welcome   messages will be randomly picked by DialogFlow when the chatbot operates.

8. Create    Custom Intent.   We   want   the    agent   to   inform.    customers   about   the   opening   hours   and   schedule   appointments   for   customers.   Create   a   new   intent   named Hours by   clicking   the   +   icon.   Then, click “Add Training Phrases”   . In the   Training phrases   section   of   the Hours   intent,   enter   the   following   training   phrase:   “When   are   you   open?”.      In   the   Responses   section,   add   “We're   open   from 9 AM to 6   PM every   day.   Is there   anything   else   I   can   do   for you?”

9. Adding more training phrases.   In natural   conversations,   we   almost   always   have   different   ways   of   forming phrases that mean the same代 写EIE1005 Fundamental AI and Data Analytics Workshop 3R
代做程序编程语言 thing. The more training phrases you provide for intent, the   more likely that user utterances are correctly matched with the intent.    Add   the   following   training phrases:
a.         Are you open today?
b.         How late are you open   on weekends?
c.         When do you   close?
d.       What time   do   you   open tomorrow morning?
e.         Are you open now?
f.            Business hours.
g.         How early can   I   drop   in?
h.         Tell me your opening hours.
i.            What are your hours?
j.            How late can   I   come in?
Click   “Save”   and try   something   similar to the   above training phrases   in   the   “Try   it   now”   edit   box.

10.      To   allow   customers   to   make   appointments,   an   Intent   should be   able   to   collect   the   date   and   time   information   from   the   customers.   To   this   end,   we   may   create   a   new   Intent   that   accepts   input   parameters. The entities and   parameters of   an Intent allow the agent to extract targeted information   from user utterances   and   convert   it to   a   set   of   parameters,   which then   can   be   processed   by   other functions or systems to perform. various tasks.Create   an   intent   named “Make Appointment”   .   In the   Training phrases   section,   add   the training   phrase: “Can   I   schedule   service for   4   PM tomorrow?” In   the   Action   and   parameters   table,   verify   that the system entity   @sys.date-time   has appeared.
In the “Text response table”, add the response phrase: “Got it.   I   have your appointment scheduled   on $date-time. See you soon. Good-bye.” Test your   new intent   by entering “Can I schedule service   for   5   PM   tomorrow?”

11. Intent with more interaction.   Sometimes users may only   provide   the   date   without   the   time.   We
could request users to provide the time in the next dialog by setting the entity as   “Required”.
Add a training phrase for date parameter:
Add + New parameter for time (you may need to add a training phrase   for time also):

Add Response for date   and time:

Try the input “May   I come on Tuesday?”, followed by   10:00 AM.

12. Integration with Dialogflow Messenger. You may make your chatbot accessible on the browser.
Click “Integrations” and select “Dialogflow Messenger”   . Then “enable” and   “Try   it   now”   .  

In-class demonstration: 
Demonstrate the Dialogflow Messenger to our TAs/Technicians and sign on the mark sheet in class.    Marks will only be given to those who signed the mark sheet. 
E. Design Your Own Chatbot 
13.             This part   is more   challenging.   If   you   are   happy   with   getting   70%   marks   in   this   workshop,   skip   this part. You should create a   chatbot   for   a   company   in   your   discipline.   For   example,   if   you   are   optometry   students,   you   may   design   a   chatbot   for   an   optical   and   contact   lens   shop.   If you   are   from Design   School, you may design a   chatbot   for   a   design   house   or   fashion   shop.   Your   marks   will depend on   your innovation and functionality of   your chatbot.   You should show in   your   report   that your chatbot works as expected. You may refer to the following links to   see more   advanced   features   of DialogFlow. Because   it   is   a 4-hour workshop, you   do not   need   to   implement   a   full- fledged chatbot.
For the report format, I encourage   you to   design   your   style.   However,   the   report   should   contain   all the results of   the workshop. Typically, a report contains the following contents:
1)       What   are the   goals?
2)       What are the   expected outcomes?
3)       Any advanced   features?
4)       The   outcomes   (results)
5)       Explanations   ofthe   outcomes   and   your   observations


         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
