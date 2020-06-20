# Hands on Lab: Classify your images with AI!
> 
> * * *
> 
> ## **Lab overview:**
> 
> ### Scenario
> 
> IBM Watson Visual Recognition (VR) is a service that uses deep learning algorithms to identify objects and other content in an image. In this hands-on lab, you will use Watson VR to upload and classify images. 
> 
> **Note:** To complete this exercise, you will create an IBM Cloud account and provision an instance of the Watson Visual Recognition service. A credit card is NOT required to sign up for an IBM Cloud Lite account and there is no charge associated in creating a Lite plan instance of the Watson VR service. Objectives
> 
> After completing this lab, you will be able to:
> 
> 1.  Access IBM Cloud
> 2.  Add resources to your IBM Cloud account
> 3.  Add services to your IBM Cloud account
> 4.  Create a project in Watson Studio
> 5.  Analyze images using Watson VR
> 
> ## Exercise 1: Create an IBM Cloud Account
> 
> ### Scenario
> 
> To access the resources and services that the IBM Cloud provides, you need an IBM Cloud account. 
> 
> If you already have an IBM Cloud account, you can skip Tasks 1 and 2 and proceed with _Task 3: Login to you IBM Cloud account._
> 
> ### Task 1: Sign up for IBM Cloud
> 
> 1\. Go to: [Create a free account on IBM Cloud](https://cocl.us/ibm_watson_visual_recognition_ai101_coursera)
> 
> 2\. In the **Email** box, enter your email address and then click the arrow.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/cUogW3LjRXKKIFty44VynQ_c3530fb8acb2f7c597f14e0119d18d3c_01_Sign_up_page1.png?expiry=1592784000000&hmac=gkvbbJO9ySGf4C7j7GbtzupZNaXTq5kz3TNLbb5LwVY)
> 
> 3\. When your email address is accepted, enter your **First Name**, **Last Name**, **Country or Region**, and create a **Password**.
> 
> **Note:** To get enhanced benefits, please sign up with your company email address rather than a free email ID like Gmail, Hotmail, etc.
> 
> If you would like IBM to contact you for any changes to services or new offerings, then check the box to accept the option to be notified by email.
> 
> 4\. Click **Create Account** to create your IBM Cloud account.
> 
> ### Task 2: Confirm your email address
> 
> 1\. An email is sent to the address that you signed up with.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/GKnjJfRNQEKp4yX0TcBCZw_591c9e79ea9f718805eaf1b40fac3187_02_Sign_up_message1.png?expiry=1592784000000&hmac=bCvUGLqvA-8dtXgQmaOD4Ye3aEdW8IzNAMzjq0hMKO0)
> 
> 2\. Check your email, and in the email that was sent to you, click **Confirm Account**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Jb1reflUQGO9a3n5VIBjKg_4f0f16bb78718a9bbdb8a45842951bee_03_Confirm_Account.png?expiry=1592784000000&hmac=DE39q-DemF6JwDdVNH1KwMLk9TmRixV8FsWuekBOWsY)
> 
> 3\. You will receive notification that your account is confirmed.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/NudS1AP1RxCnUtQD9fcQPQ_1c256b25f0aa3b51d87135318906645f_04_Welcome_msg1.png?expiry=1592784000000&hmac=T_JgygftVL1whxiLy9h3H7I07tGxJdn0ATVDcFean-M)
> 
> Click **Log In**, and you will be directed to the IBM Cloud Login Page.
> 
> ### Task 3: Login to your IBM Cloud account
> 
> 1\. On the [Log in to IBM Cloud](https://cloud.ibm.com/login) page, in the **ID** box, enter your email address and then click **Continue**. 
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/zD8D-nUVSy-_A_p1FWsv7g_f73d8fbcaebcb4fb7485196b87a89985_05_Login_1.png?expiry=1592784000000&hmac=GA1Ay1TxQmolSl8hzmJyZ0g5U9pHJRZUOu8wFq-KUWw)
> 
> 2\. In the **Password** box, enter your password, and then click **Log in**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/TXV96QqVQ6q1fekKleOq1w_7ff8303a44307b7d4c252c474a6555ad_06_Login_2.png?expiry=1592784000000&hmac=UTg_ezeu6n_E0a_G7OSTHBhVryAX0K3QIAzyd3ddf4E)
> 
> ## Exercise 2: Create a Watson Studio Resource
> 
> ### Scenario
> 
> To manage all your projects, you will use IBM Watson Studio. In this exercise, you will add Watson Studio as a Resource.
> 
> ### Task 1: Add Watson Studio as a resource
> 
> 1\. On the Dashboard, click **Create Resource**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/D5EfRscpSUaRH0bHKZlGjA_5489a00c28f342f693e50a93cc9acdc2_07_Create_Resource_1.png?expiry=1592784000000&hmac=03qZlIEyJQ4-1gLMUa6aG6TLmHJ8fGGuD3RwN5CBgJ0)
> 
> 2\. In the Catalog, click **AI (16)**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/GRhiz14fRt2YYs9eH9bdrQ_473494ffeaa90c658a8416d785b74bd7_08_Catalog.png?expiry=1592784000000&hmac=eCEjX6wGIrKNJ4cGQ2Hl4zE2sMcopPXitCTeSbCDh4Q)
> 
> Note that the **Lite** Pricing plan is selected.
> 
> 3\. In the list of **Services**, click **Watson Studio**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Y5oc9qV2QdyaHPaldiHcOA_ad73106f5cd0d8946028e67dff0d2e4d_09_Watson_Studio_Catalog.png?expiry=1592784000000&hmac=_V6nNr52B8lGHMI5SC0Wbajr8zkJ0xvO8lGQ7iV9oFU)
> 
> 4\. On the Watson Studio page, select the region closest to you, verify that the **Lite** plan is selected, and then click **Create**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Dgsh6DX8RiGLIeg1_PYhZw_4dc86d3f3ebd8f4d9a502fbaa97530c3_10_Watson_Studio_Lite_sign_up_2.png?expiry=1592784000000&hmac=kBQlKZbmkeGapTeDz6fuaYYoCfXl1ADn9ZnrAVfknXo)
> 
> 5\. When the Watson Studio resource is successfully created, you will see the Watson Studio page. Click **Get Started**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2FxbBXtzQaucWwV7cxGrwQ_303f9c7c035852d4b258069267cb4665_11_Watson_Studio2.png?expiry=1592784000000&hmac=oYB8RtWBCNiG5WxGxxh0VCXbGzq1MlSpRTvI2axBbNs)
> 
> 6\. You will see this message when Watson Studio is successfully set up for you.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/QtfNpH9bR7uXzaR_W4e7YQ_7e0fa28f89e80f8f136393de9ab1fee7_12_Watson_apps_ready.png?expiry=1592784000000&hmac=BChNYaOjlqn9cGf1Np-07dC_wV1MF0LzijfsAr2IZGI)
> 
> ## Exercise 3: Create a project
> 
> ### Scenario
> 
> To manage all the resources and services that you are working with, you should create a Watson Studio Project. You will begin by creating an empty project, and then adding the resources and services that you need. 
> 
> ### Task 1: Create an empty project
> 
> 1\. On the Watson Studio Welcome page, click **Create a project**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/98WfBitzRvOFnwYrc4bzOw_3bd96428a21b1c76f73be9b15b39d9d7_13_Create_project_3.png?expiry=1592784000000&hmac=LC33rXCP9G9CfiHyfz67lz6dD8rn2pD50v4KMwnciys)
> 
> 2\. On the Create a project page, click **Create an empty project**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/IZGXL9POR0SRly_TzqdEfg_d48e79305f8895c8f8d3954b033e792f_14_Create_project_5.png?expiry=1592784000000&hmac=gFQnL31zszSTNegCiCSOCo9oFz3UQmM6P2nKYf2_1uM)
> 
> 3\. On the New project page, enter a **Name** and **Description** for your project.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/pwOefhlsQGaDnn4ZbMBm-Q_7e6e17db7f7110f0fa0b3f94278c5b92_15_New_Project_details_2.png?expiry=1592784000000&hmac=wE0kXArbOgEbjcxYeOw3D4KkjeiLh9ntZ47f5aC-ls8)
> 
> 4\. You must define storage for your project before you can create it. Under **Select storage service**, click **Add**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/EsfR-G1QQWeH0fhtUIFn2g_53ed199fde85fab0f92a58656e4e2f77_16_New_Project_details_3.png?expiry=1592784000000&hmac=q1qOIVujFgw7uuDis6IosbaKaL2zH0uy1uT3V7rpMk4)
> 
> 5\. On the Cloud Object Storage page, verify that **Lite** is selected, and then click **Create**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/0-0Djp8pShCtA46fKboQ2Q_767199fdcb4ee332f9a311bc3b3adbec_17_Select_storage_2.png?expiry=1592784000000&hmac=fTjHEIGcKYWsSdb5toaSUcjeWi8na6HxRqGiCPQwUNU)
> 
> 6\. In the Confirm Creation box, click **Confirm**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jLA6FljGSzywOhZYxos87A_ab3064f07864cde8c58f370c0f62174f_18_Confirm_Creation_2.png?expiry=1592784000000&hmac=Bj-3RBHnYOLZ2g9q4dtvAisPEhKVegIuLe45c6Dt_5s)
> 
> 7\. On the New project page, under **Define storage**, click **Refresh**, and then click **Create**.
> 
> ## Exercise 4: Add a Watson VR Service instance
> 
> ### Scenario
> 
> This project will focus on analyzing images, so you need to add the Watson Visual Recognition Service. You will also need some images to analyze, so follow the setup steps below to ensure you are prepared.
> 
> ### Setup
> 
> Before you begin this exercise, you must complete the following steps:
> 
> 1.  Collect a set of at least 20 images. You can use your own images, or download them from the internet. 
> 2.  Store the images in an easy to find location.
> 
> ### Task 1: Add the Visual Recognition Service
> 
> 1\. To add services to the project, click **Add to project**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/wLSDTx9qS5S0g08fanuUqw_17aef54e688a6bbc5768966a243773fd_19_Add_to_Project_3.png?expiry=1592784000000&hmac=bjWwYtowz5Dj1Fowdkid1qnfmckcOZz7a6W5xC5h1BI)
> 
> 2\. In the Choose asset type box, click **Visual Recognition**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vdedJL5WQbqXnSS-VhG6Uw_9031fd48ac39c11d3758b638976fb4d1_20_Add_VR.png?expiry=1592784000000&hmac=Zr6oEcU5qM9KNssQ53s5j0-hlal16x85or4yKLWz0XY)
> 
> 3\. In the Associate a service box, click **here**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/86nnjZdmT06p542XZl9O5A_8a9600a2e7067eadf36f0dbb1bfd6783_21_Associate_Service.png?expiry=1592784000000&hmac=V3qCE41T9b2azxcAyA43C7sfk9Fk7R2BGhPTCZN7uIE)
> 
> 4\. On the Visual Recognition page, verify that **Lite** is selected, and then click **Create**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/b9ZktapcTG6WZLWqXJxuoA_e77c726db57189b49fe92f214e3ba34a_22_Visual_Recognition_Create.png?expiry=1592784000000&hmac=lt87CVRn4UgXxDiWlolCN7gX5jV4m8_v-HVqlJsD7FY)
> 
> 5\. In the Confirm Creation box, click **Confirm**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/cVCWyBuaRCiQlsgbmsQoSg_5ea7f37188e9eeea0ad92b6b61f95fc8_23_VR_Confirm_Creation.png?expiry=1592784000000&hmac=H5X6_sErgLCE1_JXG_nEbR7gnCn3lCIHxGwaO2820m8)
> 
> ### Task 2: Analyze images with Watson VR
> 
> Now you can see all the built-in image classification models that IBM Watson provides! Let's try the General model.
> 
> 1\. To analyze your images, on the Models page, under **Pre Built Models**, in the **General** box, click **Test**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/-frWxgL2QL661sYC9jC-MQ_2eda9174e44aecb838e0b654b48e9618_24_VR_Models.png?expiry=1592784000000&hmac=xe44t0dkFWUdGtxQh0dRsbpeHGmwznzdti1h3JoHM9w)
> 
> 2\. On the General page, click the **Test** tab.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/NIosFV2PSKCKLBVdj-igjA_55177ce011a2a91c007954f46b7e85e2_25_General_page_Test.png?expiry=1592784000000&hmac=mMMYA-rn45cF5bmT6w4Uec_UYjkhrOFbe2PldLHUSMA)
> 
> 3\. To upload images, on the Test tab, click **Browse**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/oItMdyLBTRKLTHciwe0SAw_5606ae0b6fd8d9065b2cb7c46c6babc8_26_Test_Browse_for_images.png?expiry=1592784000000&hmac=bU_cTUR2Iemc0PNTJKdhHTv_oNNs6SthDXMqgx8S7Bs)
> 
> 4\. Select the images you want to upload and then click **Open**.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/nenb8X-KTFmp2_F_ijxZ_A_1f6dd65a96d40691b04c6bb2adbc4351_27_Select_images.png?expiry=1592784000000&hmac=aPV09T9kyautvfXK8EQApR-EN5uhzKjbtpz0-GUE_ds)
> 
> 5\. Once you have uploaded your images, Watson Studio Visual Recognition will tell you what it thinks it found in your images! Beside each class of object (or color, age, etc.), it gives you a confidence score (between 0 and 1) showing how confident it is that it found that particular object or feature in your image (0 for lowest confidence and 1 for highest confidence).
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/lkRLHNZgRPaESxzWYJT2gw_597c46ae54adfbc2348e5b31c03b66db_28_Uploaded_images.png?expiry=1592784000000&hmac=_1dRP9YLt90roHWHZLjV2fHzFtLAHQiu2iqWWz-WE0Y)
> 
> 6\. Use the check boxes on the left to filter the images. In this example, only images in which Watson VR has detected **beige color** are displayed.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/_0mBlYgWQ3mJgZWIFuN5vQ_6aa446e2076ae71145b46fefaff51522_29_beige_images_only.png?expiry=1592784000000&hmac=PFpD0pKihCP9aEQEHW-AVsi6LD_m8_hsnLQhT86TK0c)
> 
> 7\. Use the **Threshold** slider to only display images in which Watson VR has at least 90% confidence of the beige color.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/dcFo0yyxQNqBaNMsscDa_Q_39235b678895a0c7827826bda2ae7f76_30_High_confidence_in_beige.png?expiry=1592784000000&hmac=NP1uZPF3dhH87jUaLYd_Nu4ZPBG-e4KNcFOR87bgOjw)
> 
> ### Task 3: Save a screenshot
> 
> **Note:** The screenshot saved in this step will be required as part of the Graded Final Assignment for those pursuing a certificate for this course. This step is _optional_ for those auditing the course.
> 
> 1\. From Task 2, choose just one of the images that you uploaded. Select an image that does not have too many classes of objects. 
> 
> 2\. Take and save a screenshot in .jpeg or .jpg format including the Watson Visual Recognition confidence scores (that are indicated below the image). Ensure the labels and confidence scores below the picture are readable. See the  sample screenshot below.
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/R2dCo6qHRaSnQqOqh1Wkeg_c6c9bf2b9393693764ebe046c01f18b9_30a_Sample_Screenshot.png?expiry=1592784000000&hmac=ssFmrBhNEiFdvRxxaq0JRTvc1h3hoIwFBlh3J4nc3YA)
> 
> ### Task 4: Share your results
> 
> Follow us on Twitter and send us some of the funniest and most interesting results you found with IBM Watson Visual Recognition!
> 
> ![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/47Q6Ae5iSRG0OgHuYgkRFA_0aa2cbe5f29718384b4af46b553d7b6d_31_Suggested_Tweet.png?expiry=1592784000000&hmac=Ht1bAo3zTxXOi6POOxRrfDpH4xWVtfF2BRMs9LTZpak)
> 
> [Click here](https://twitter.com/intent/tweet?text=I%20just%20learned%20how%20to%20use%20Artificial%20Intelligence%20to%20classify%20images%20with%20@IBMWatson%20in%20this%20Introduction%20to%20AI%20course%20by%20@ravahuja%20on%20@Coursera%20-%20https://www.coursera.org/learn/introduction-to-ai) to share the above Tweet.
> 
> [Follow Rav Ahuja](https://twitter.com/ravahuja)
>
> -- https://www.coursera.org/learn/introduction-to-ai/supplement/TRj8u/hands-on-lab-classify-your-images-with-ai#main
