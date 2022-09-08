<h1 align="center">Follower Network</h1>
A network graph consisting of nodes and edges displaying centrality between Twitter accounts that follow @PlayValorant Twitter account.
 
## 📇 Details 
The source of the network data comes from the Twitter API (developer.twitter.com). From retrieving the data using the Twitter API, I set the target Twitter account to @PlayValorant. I then proceeded to enable the code to look throughout the first 50 friends of the account and then the first 50 of the already checked accounts. By collecting data in this way, it can be determined if the friends selected have a connection with each other based on the following status. The nodes in the network represent the different entities of the first 50 friends and the edges represent the connection the friends have with each other (following status). After I gather this data, I checked to see how many total nodes and edges were represented in the graph. The network resulted in 1528 nodes and 1869 edges.

## 🚫 Limitations
The limitations for this project include the lower disk reading speed and lowered runtime for Google Colab. Due to the lower disk reading speed, it took a long time to read in the data meaning the API could only read in a certain amount of data for the limited runtime. My main takeaway is that people of similar interests are much more likely to follow each other and the main account. For example, in this case, people who are content creators for the game were more likely to be friends while at the same time, following the @PlayValorant Twitter account.

## 🧗 Challenges
One bug I encountered is getting the data to process the first few (50) friends of the accounts. I made a mistake making a while look instead of for loop. Having the code written as a while look, the amount of friend count would exceed what was initially set as it became an infinite loop due to improper counter. By using my critical thinking skills, I quickly decided a for loop would be much more efficient and easier to deal with. While working with the for loop, the code was taking a longer time to finish executing due to the number of friends that was set to the variable of friend amount. To solve that issue, I lowered the friend count to 50 which was initially set to 100. Data cleaning-wise, there wasn’t much to do. The framework, Tweepy, already gave out clean data which were just Twitter accounts. All I had to do is retrieve the 50 accounts and set them into nodes and edges using the NetworkX framework.

## 👷 Built With

![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)

![image](https://img.shields.io/badge/VSCode-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)

![image](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

## 📚 Libraries

- [x] NetworkX
- [x] Gephi

## 🧑🏻 Author

**Teja Tammali**

<a href="mailto:tejat18@umd.edu"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a> 

[![name](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/tejatammali/ "Welcome to my Linkedin!")

[![name](https://img.shields.io/badge/Medium-12100E?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@tejat "My Medium Profile")
