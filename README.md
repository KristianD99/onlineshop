![onlineshopPic1](https://github.com/KristianD99/onlineshop/assets/136342597/a35acd28-71f9-4a99-a867-c149980ebd0c)

![onlineshopPic2](https://github.com/KristianD99/onlineshop/assets/136342597/9850ff23-cb68-4c63-869c-965e64c32e76)

![onlineshopPic3](https://github.com/KristianD99/onlineshop/assets/136342597/e2e29a0f-ce13-4df6-bd42-8e2802bcb2d6)

![onlineshopPic4](https://github.com/KristianD99/onlineshop/assets/136342597/06a0cf3c-6258-4573-b41b-57b9544183f1)


OnlineShop Website using MERN stack

  
        - Reactjs
        - Material UI
        - Redux
        - Typescript
        - Cors
        - Stripe
## Getting started
This server project needs an environment file. To get it you will need to create a file named `.env` in the root dir of this project. If all is correct it ought to be above package-lock.json. In it you will need to set up a MongoDb url. To get this, visit the mongo DB website [here](https://www.mongodb.com/cloud/atlas/register). We recommend that you sign up using Google as it is faster. 

Then once this is done, you need to add a Db cluster by clicking the __add db cluster__ button. Then pick sandbox and an appropriate provider and region. For Europe we recomend __AWS__ at the __Frankfurt__ region on a __shared__ resource type.

![MongoDB setup screen](image-1.png)

__IMPORTANT__ This website might ask you to add your current IP in order to get conected. Please do so, otherwise errors may occur. 

Then create a username and password to connect to your DB (again using that UI) and make sure you store these. 

Once the db is deployed you can click on connect

![Open up I to conenct to the DB](image-2.png)


and then pick the first option, named __drivers__. After that you need to copy the URL, which looks like this `mongodb+srv://dbadmin:<password>@cluster0.q1frpai.mongodb.net/?retryWrites=true&w=majority` and replace the `<password>` bit with you password. 

Example: 

If your password is `123456`, and your username is `admin`, then the url will be `mongodb+srv://dbadmin:123456@cluster0.q1frpai.mongodb.net/?retryWrites=true&w=majority`

Once this is all done, just paste this line in your `.env` file
`MONGO_URL= <THE MONGO URL YOU HAVE JUST MADE>`

Your app now knows how to connect with mongo!

Next up is to add anoher three values in the `.env` file, these are:

```
CRYPTOJS_SECRET = <A RANDOM STRING>
JWT_SECRET = <A RANDOM STRING>
CRYPTO_KEY = <A RANDOM STRING>
```

With this setup you can now move to the final part of the environment setup and that is `stripe`. 

