# Songs_Suggesting_System_Using-_chatbot

In this project we, would be combining multiple services and open-source tools to make a chatbot that suggest’s song based on the tone of the conservation on which the user is having with the Chatbot. It could live in any major chat applications like Facebook Messenger, Slack, Telegram, Text Messages, etc.

We would be building an extensive Chatbot service, to which we can talk to. And talking to a chatbot wouldn't be business-driven. It would just be casual conversations. Further, on top of it, the chatbot would also be suggesting songs to the user based on the tone of the user. This song suggestion feature is  the use of Last.fm API, very much similar to the popular Spotify API. Also for tone/emotion analysis of the conversation we will be using the IBM Tone Analyzer API.

Collaborating with these types of APIs is very much critical as in today's world the popular chatbots do much more than simply having a data-driven conversation to supplement additional user-oriented features. Also the reason to choose python to build the chatbot is because python boasts a wide array of open-source libraries for chatbots, including scikit-learn and TensorFlow.

In this area of technological advancements, songs suggestion based on mood is much needed at it will help humans relieve stress and listen to song’s according to their mood.

In this project, we have implemented a chatbot that suggests songs based on the user's text tone. By analyzing the tone of the text expressed by the user, we can identify the mood. Once the mood is identified, the application will play songs in the form of a web page(ANVIL) based on the user's choice as well as his current mood.
 
	


                                                                              #Abstract
                                                                              
                                                                              
In this project we, would be combining multiple services and open-source tools to make a chatbot that suggest’s song based on the tone of the conservation on which the user is having with the Chatbot. It could live in any major chat applications like Facebook Messenger, Slack, Telegram, Text Messages, etc.
We would be building an extensive Chatbot service, to which we can talk to. And talking to a chatbot wouldn't be business-driven. It would just be casual conversations. Further, on top of it, the chatbot would also be suggesting songs to the user based on the tone of the user. This song suggestion feature is  the use of Last.fm API, very much similar to the popular Spotify API. Also for tone/emotion analysis of the conversation we will be using the IBM Tone Analyzer API.
Collaborating with these types of APIs is very much critical as in today's world the popular chatbots do much more than simply having a data-driven conversation to supplement additional user-oriented features. Also the reason to choose python to build the chatbot is because python boasts a wide array of open-source libraries for chatbots, including scikit-learn and TensorFlow.
In this area of technological advancements, songs suggestion based on mood is much needed at it will help humans relieve stress and listen to song’s according to their mood.
In this project, we have implemented a chatbot that suggests songs based on the user's text tone. By analyzing the tone of the text expressed by the user, we can identify the mood. Once the mood is identified, the application will play songs in the form of a web page(ANVIL) based on the user's choice as well as his current mood.
 
 
 
List of Tables

Table: 01	Backend Tools/Software	2

Table: 02	Frontend Tools/Software	2



Table of Contents
Declaration	(i)
Certificate	(ii)
Acknowledgement	(iii)
Abstract	(iv)
List of Tables	(v)
Chapter 1: Introduction	1
    1.1. Overview	1
    1.2. Requirement 	2
        1.2.1 Backend tools	2
        1.2.1 Frontend tools	2
    1.3. Architecture of  Project 	2
Chapter 2: Methodology 	3
    2.1. Methodology	3
        2.1.1 Chatbot and Architecture	4
        2.1.2 Emotion Detection IBM	9
        2.1.3 Last.fm API	11
    2.2 Anvil Editors Architecture 	14
Chapter 3: API Testing	16
      3.1 Postman Version-9.18.3	16
      3.2 Emotion API Testing	17
Chapter 4: Project Demonstration	18
     4.1 Homepage  	18
     4.2 Chat With Chatbot	20
     4.3 Review Page  	22
     4.4 Team Page	23
Chapter 5: Conclusion and future scope	24
    5.1. Conclusion	24
    5.2. Future Scope	24

References 	25
	
 
                                                           Chapter 1 : Introduction

1.1	Overview:
This Project is aimed to implement a song based web application to assist user and provide a more personal experience.
This Project includes chatbot which will be trained  by combining multiple services and open source tool’s to simulate a human conversion to suggest songs based on the tone of the conversion.
The purpose of chatbot is to support and scale business teams in their relations with customers,it could live in any major chat applications like Facebook Massenger ,slack,Telegram,Text messages,etc.
This project is focused on building a custom chatbot that will be our fundamental step of the learning curve of building our own professional chatbots. 
In this project ,we would be building an extensive chatbot service ,to which you can talk to and talking to a chatbot would not business-driven . 
The suggestion feature is the use of last.fm API,very much similar to the popular spotify API  & for tone/emotion analysis of the conservation we will be using the IBM Tone Analyzer API. 
Collaborating with these types of API is very much critical as in today’s world the popular chatbots do much more than simply having a data-driven conversation, to supplement additional user-oriented features .Also the reason to choose python to build the chatbot is because python boasts a wide array of open source libraries for chatbots ,including Keras and TensorFlow .
It is great for small data sets and more simple analysis , also python’s libraries are much more practical.



1.2	 Requirement: 

1.2.1 Backend tools :-

Sr.	                       Analysis 	    Software/Tools
01.	                Song’s Suggestion     	Last.fm songs API
02.                	Emotional Analysis  	IBM Tone Analyzer API
Table.1
 
1.2.2 Frontend tools: -

Sr.	                       Analysis	             Software/Tools
01.	                 User Interface            	Anvil Framework
02.                    	Language	                 Python-3                           
03.                   	Run On 	              Google Colaboratory                                          
04.	                   Testing API	         Postman Version-9.18.3
Table.2

1.3	Architecture of project:
 
                                                                  
User starts the conservations. .
	Emotional Analysis of the conversation is done using the IBM Emotional API. 
	Get the reply to the conservation from the chatbot. 
	Based on the Emotion which the app perceives ,top songs are retrieved using Last.fm songs API. 
	If the user listens to a particular song for sometime similar song would be suggested to the user Last.fm API.
	Finally We will getting Our Desired output.


                                                            Chapter 2 : Methodology

2.1	Methodology:- 
 
 	“Song Suggesting System” is basically a web app which is used to suggesting songs based on conversation with users. Our web app is primarily a chatbot which holds a conversation with the user.
 	In the next step that conversation is analyzed by an emotion detection module to determine the mood of the user. Further the music will be suggested on the basis of the emotion of the user. 
 	Three main modules of the web app are - Chatbot , Emotion Detection and Songs suggestion.
 	In the Next step , We have Import and load the data file in Google colaboratory.
 	After Loading the data we have Extracting and Preprocessing data.
 	After preprocessing data we have Created a Training Data.
 	After Training data we have Developing  our Model.
 	After the model gave the class it belongs to, we implemented some functions to identify the class and then retrieve a random response from the list of responses.
 	After predict the response  we have Analyse the tone this will determine the emotion of conversation between user and chatbot through IBM Tone Analyzer API.
 	After Analyzing the tone of user  we used the Last.fm Songs API so that we can suggested some songs to the user based on the tone/emotion of the user.
 	By the end, we got 5 top song recommendations based on the emotion of the user.




2.1.1	Chatbot:

  

•	A chatbot is a software application used to conduct an online chat conversation via text or text-to-speech, its providing direct contact with a live human agent. 

•	We can also say that, chatbot is an intelligent piece of software that is capable of communicating and performing actions similar to a human. 

•	It provides an interactive platform to communicate with users.

•	Chatbots have varying levels of complexity, being either stateless or stateful. Stateless chatbots approach each conversation as if interacting with a new user.

•	In contrast, stateful chatbots can review past interactions and frame new responses in context.
•	Adding a chatbot to a service or sales department requires low or no coding.
•	Many chatbot service providers allow developers to build conversational user interfaces for third-party business applications.
•	In this project we created a simple chat bot that will be used to answer frequently asked questions. 

Chatbot Architecture: 
Chatbot architecture is the spine of the chatbot. The type of architecture for our chatbot depends on various factors like use-case, domain, chatbot type, etc. 
However, the basic conversation flow remains the same. Let us discuss more about the critical components of chatbot architecture:

 
1)	Question and Answer System:
As the name suggests, the Q&A system is responsible for answering customers’ frequently asked questions. The question is interpreted by the Q&A system, which then replies with appropriate responses from the knowledge base.

It consists of the following elements:
	Manual Training: Manual training entails the domain specialist compiling a list of commonly asked user questions and mapping out the answers. It enables the chatbot to identify the most relevant questions’ answers rapidly.
	Automated Training: Automated training entails sending business documents to the chatbot, such as policy documents and other Q&A type documents, and instructing it to train itself. From these documents, the engine generates a list of questions and responses. The chatbot would then be able to respond with confidence.
2)	Environment:-
The environment is mainly responsible for contextualizing users’ messages using natural language processing (NLP).
The NLP Engine is the central component of the chatbot architecture. It interprets what users are saying at any given time and turns it into organized inputs that the system can process. The NLP engine uses advanced machine learning algorithms to determine the user’s intent and then match it to the chatbot’s supported intents list.
NLP Engine has two components:
•	Intent Classifier: An intent classifier maps between what a user asks and the type of action performed by the software.
•	Entity Extractor: The entity extractor is responsible for identifying keywords from the user’s query that helps determine what the user is looking for.
An NLP engine can also be extended to include feedback mechanism and policy learning for better overall learning of the NLP engine.

	Feedback Mechanism: This includes the feedback for the chatbot provided by the users. This part of learning can be incorporated into the chatbot itself. Here, the user rates the interaction at the end of the conversation. It encourages the bot to learn from its mistakes and improve in future interactions.
	Policy Learning: Policy learning is a broad framework wherein the bot is trained to create a network of happy paths in the conversation flow that increase overall end-user satisfaction.

3)	Front-End Systems:- 

Front-end systems are the ones where users interact with the chatbot. These are client-facing systems such as – Facebook Messenger, WhatsApp Business, Slack, Google Hangouts, our website or mobile app, etc.
4)	Node Server / Traffic Server:-
It is the server that deals with user traffic requests and routes them to the proper components. The response from internal components is often routed via the traffic server to the front-end systems.
5)	Custom Integrations
With custom integrations, our chatbot can be integrated with our existing backend systems like CRM, database, payment apps, calendar, and many such tools, to enhance the capabilities of our Chatbot.




2.1.2	Emotion  Detection – IBM:

 
                                                                             

In this  project ,we would be Also used the IBM Tone Analyzer API so that we can analyse the tone of conservation(emotion).
 We are using an API here as we don’t have that enough data , Computational power and time to create our own model API. 
Tone Analyzer services uses linguistic analysis to detect emotional and language tones in written text IBM Analyzer emotions and tones in what people write online, like tweets or reviews . Predict whether they are happy , sad , confident and more .
IBM also enhance customer service monitor customer service and support conservation so you can respond to our customers appropriately and at scale .See if customers are satisfied or frusted , and if agents are polite and sympathetic .
 IBM also help if our chatbot enable to detect user tones so you can build dialogue strategies to adjust the conversation accordingly.

After running the code, tone Analyser Service, we would have the analysis of the text on our system which looks similar to this. Here as the top is the tone of the entire app and below is the tone of every sentence-



 



2.1.3	Last.fm API: 

API(Application Programming Interface): 

           
API (Application Programming Interface) is a set of functions that allows applications to access data and interact with external software components, operating systems, or micro services. 
API lets a developer make a specific “call” or “request” in order to send or receive information. This communication is done using a programming language called “JSON.”  It can also be used to make a defined action such as updating or deleting data. There are four basic request methods that can be made with API:
1.	GET – Gathers information (Pulling all Details)
2.	PUT –  Updates pieces of data (Updating category)
3.	POST – Creates (Creating a new Category)
4.	DELETE – (Deleting a post)


JSON (JavaScript Object Notation) is used to represent data on a server. It’s fairly easy to read by humans, and easy for machines/applications to understand. 

 






Let’s Discuss About last.fm API: -


	
In this Project, we would Also be used the Last.fm songs API so that we can suggested some songs to the user based on the emotion of the user. 
API is the acronym for application programming interface , Which is a software intermediary that allows two applications to talk to each other. 
Each time we use an app like Facebook , send an instant message , or check the weather on our phone , we are using an API.




2.2	       Anvil Editor Architecture:

 


The anvil editor , provides the full functionality required for developers to design,build and ship web apps in minutes. 
They only need to know one language -python – to create powerful,fully functional apps.over 8 million people can program in python ,opening up web development to a wider range of people, such as data scientists, frontend developers and also backend developers and making it faster and simpler.
 Anvil development environment combines coding simplicity with the power of python , allowing the creation of full stack web apps in minutes bringing the spirit of classic RAD tools like visual basic to the modern web.
there are no limits on the scope of the apps created – the ability to code in python delivers industrial- strength flexibility and scalability, and a best ecosystem of python libraries and tools.
This is free  Online  very  good &  Interesting tool anyone can use it, without any cost.


                                                         Chapter 3: API Testing

3.1 Postman Version -9.18.3: 
                            

•	Postman is a computer application used for API testing.
•	Postman sends an API request to the web server and receives the response, whatever it is.
•	No extra work or setting up of framework is required while sending and receiving requests in Postman.
•	Its Extensively used by Testers and Developers for better testing of application. Easy to integrate with Continuous Integration (CI) & Continuous Development Pipeline.



3.2 Emotion API testing:-
Step 1: Open The Postman.
Step 2: Copy API key From (Google Colabatory ).
Step 3: Paste into Postman key url.
Step 4: Set Postman As  “GET”  Details of API.
Step 5: Click On “SEND” , Then it will give me details of this API.
Step 6: we can also Seen here like’s  parameters, header, body and limit.
After Checking API, postman will looks like-
 


                                                        Chapter 4 : Project Demonstration

In this project We have Demonstrate with 4 main button given As
•	Homepage Song Suggesting System
•	Chat with chatbot
•	Review page
•	Team Page
Now let’s Discuss one by one-
4.1    Homepage: 
      After running the application, then my Homepage is looks like given below - 
 


4.2  Chat With chatbot: 

We can also chat with our chatbot , after chatting with chatbot my application is give me suggestion for listening   song’s  as per the mood of user (in my case you can clearly see that in below figures, the user mood is “Joyfull”), this songs will comes through to last.fm api, as shown in below figure- 
   

When We Click On Any Tracks whatever we want  then it will redirect to me on this song through to Last.fm API. As shown in below figure : 
 



4.3 Review Page: 
This is Important part of My project, “review page”, user can also give me feedback through this form.
 




4.4 Team Page: 
In this whole project Contribution is done by two members as shown below in figure-
 





                                                       Chapter 5: Conclusion & Future Scope

5.1 Conclusion:
Chatbots are one of the most important advancements of AI Technology. Our project successfully combines this technology with the humans need for entertainment in the form of Songs. In this age and time of technology, such an application would serve the purpose of helping humans relax and relieve their stress. The moodBot application developed in our project is a simple chatbot that allows users to choose Songs according to their mood. 
The application is implemented as a web application, thereby being available to the user whenever required. When the user chooses the song option, songs appropriate to his mood are played. the application(Last.fm) opens a specially designed website that suggests songs to him as per his current mood.
Other enhancements could be a fully functioning websites dedicated to suggest songs depending on the mood and also previous choices of the user. Also, could add like and dislike options to the songs being played so that the users liked songs are played often and the disliked songs are not played.
Our song suggesting system using chatbot is suggests songs to the user based on their mood. 
With this experiment, we can conclude that if we add the songs genre information in our app, it will increase the quality of song suggestions and we can add more features into the app to make the overall performance better.

5.2 Future Scope:
In the future , we would like to try the following things:- 
	Using audio frequency to suggested songs. 
	Trying content based algorithm. 
	Trying clustering techniques to suggested songs.
	Making the recommender system a real-time system. 





References

[1] "Collaborative filtering for music recommender system", 2017 IEEE Conference of Russian Young Researchers in Electrical and Electronic Engineering (EIConRus), pp. 548-550, 2017 (E. Shakirova)

[2] "Music recommender System," 2nd ed., vol. 3, Brach Shapira, Ed. New York: Springer, 2015, pp. 453-493. (Music recommender System, 2015)

[3]  Linden, G., Smith, B. and York, J. (2003). Amazon.com Recommendations Item-toItem Collaborative Filtering. [ebook] Available Online at: https://www.cs.umd.edu/~samir/498/Amazon-Recommendations.pdf . (Linden G., Recommendations Item-toItem Collaborative Filtering, 2003)

[4] (Chatbot Song Recommender System , International Journal of Emerging Technologies and Innovative Research, 2021) at (www.jetir.org | UGC and issn Approved), ISSN:2349-5162, Vol.8, Issue 12, page no. ppd222-d226, December-2021, Available at - http://www.jetir.org/papers/JETIR2112328.pdf

[5] McFee, B., BertinMahieux,T., Ellis, D. P., Lanckriet, G. R. (pp. 909916).ACM: https://dl.acm.org/doi/abs/10.1145/2187980.2188222 (The million song dataset challenge. In Proceedings of the 21st international conference companion on World Wide Web, 2012)

[6] Gershman, A. and Meisels, A. A Decision Tree Based Recommender System. [eBook] IEEE Xplore, pp.170-179. Available at: https://subs.emis.de/LNI/Proceedings/Proceedings165/170.pdf .[Accessed Dec. 2, 2007]. (Gershman, 2015)

[7] DOI:https://doi.org/10.1145/3038912.3052569 (Xiangnan He, Lizi Liao, Hanwang Zhang, Liqiang Nie, Xia Hu, and Tat-Seng Chua. 2. Neural Collaborative Filtering. In Proceedings of the 26th International Conference on World Wide Web (WWW '17). International World Wide Web Conferences Steering Committee,) 

[8] (Everyone listens to songs, but how we listen is changing.) [online] Available at: 
https://www.nielsen.com/us/en/insights/article/2015/everyone-listens-to-music-but-how-we-listen-is-changing/  

[9] Bracha Shapira, Francesco Ricci, Lior Rokach: Recommender system handbook, Second Edition  Springer, 2015. (Bracha Shapira, 2015)

[10] Lhuillier, N., Bonnefoy, D., Bouzid, M., Millerat, J., Picault, J., Ribiere, M.: A recommendation system and method of operation therefore. Patent application WO2008073595 (Operation, 2006)

[11] (Theosaksomo & Widyantoro, Conversational Recommender System Chatbot Based on Functional Requirement, 2019)








#Project Submitted By:- 

Mr.Sheelaj_Babu

Mr.Anurag Singh

College:  Indian Institute Of Information Technology Bhagalpur.
