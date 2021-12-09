# Introduction

*Guangyuan Gao, Yanlin Shi, He Wang*

With the advancements of telematics technology, insurers can collect detailed car driving information. Traditionally, insurers use classical actuarial risk factors to classify policyholders and charge different premiums for different risk groups. 
Telematics car driving data is a very personalized data which encodes driving differences not contained in  classical social-demographic risk factors such as regions and ages.
For example, some young drivers may have a cautious driving style, while some matured drivers may still have a wild and aggressive driving behavior.

In this project, we explore first steps on how such information can be learned from telematics car driving data. 
Our ultimate goal is to improve auto risk classification models by using telematics car driving data. 

Although there are concerns with using personalized  data and algorithmic prediction (Mahapatra, 2019; Cevolini and Esposito, 2020), we prefer the statement by Cather (2020) that incorporating telematics data into auto insurance risk classification systems would  "minimize insurance discrimination and increase cream skimming adverse selection".

Telematics car driving data analysis is far from being trivial because the data comes with all its challenges such as big data (we typically have TBs of data that needs to be processed), data error, etc. 
According to the current actuarial literature, among others, there are three options to learn from telematics car driving data: 
(a) Weidner et al. (2016, 2017) extract covariates from time series of telematics data using discrete Fourier transforms; 
(b) Huang and Meng (2019), Paefgen et al. (2014) and Verbelen et al. (2018) calculate summary statistics of telematics data; 
(c) Gao et al. (2020) apply convolutional neural networks to learn  patterns in speed-acceleration heatmaps. Those papers research on driving styles. 

Another stream of literature study risk exposure of driving distances or time exposures; see  Ayuso et al. (2016a,b), Boucher et al. (2017), and Lemaire et al. (2016). Telematics data is a posterior experience and  Denuit et al. (2019) propose a credibility model to incorporate the posterior information of driving behavior. Guillen et al. (2020) study the association of telematics car driving data with near-miss events such as cornering, braking, and accelerating. Geyer et al. (2020) study the effect of driving behavior on risk and insurance selection. Richman (2020) discuss possible approaches to analyze telematics car driving data.

Our data is collected by on-board diagnostics (OBD) systems rather than smartphones. There are several works on smartphone-based telematics in the IEEE Transactions journals. Wahlström et al. (2017) summarize researches on smartphone-based vehicle telematics such as vehicle navigation, driver classification, road condition monitoring. Wahlström et al. (2018) study fusion of OBD and GNSS measurements of speed.  Wahlström et al. (2015) detect dangerous cornering using GNSS data. 

The qualities of the IEEE conference papers on telematics car driving data are quite mixed. Among others, Savelonas et al. (2020), Girma et al. (2019) and Carvalho et al. (2020) apply recurrent neural networks to identify drivers or to learn different driving behaviors such as normal, moderate, aggressive, etc.

In transportation field, Joubert et al. (2016), Ma et al. (2018), and Hu et al. (2019) study driving behaviors  and find certain driving behaviors are more related to at-fault accidents.
They use both telematics data and contextual data such as road conditions, traffic flow, speed limits.
Ho et al. (2014), Hung et al. (2007), Kamble et al. (2009) study  telematics data and driving cycles to understand vehicular emissions, energy consumption and impacts on traffic in different cities of the world.

According to the current literature, we list two public telematics car driving data sets: naturalistic driving study dataset and  UAH-DriveSet (Romera, 2016). Some of the above literature is based on the two data sets. Unfortunately, our telematics data is not publicly available. 

<!-- Spectral features -->

**References**

Ayuso, M., Guillen, M., Pérez-Marín, A.M. (2016a).
Telematics and gender discrimination: Some usage-based evidence on whether men's risk of accidents differs from women's.
*Risks* **4/2**, article 10.

Ayuso, M., Guillen, M., Pérez-Marín, A.M. (2016b).
Using GPS data to analyse the distance traveled to the first accident at fault in pay-as-you-drive insurance.
*Transportation Research Part C: Emerging Technologies* **68**, 160-167.

Boucher, J.-P., Côté, S., Guillen, M. (2017).
Exposure as duration and distance in telematics motor insurance using generalized additive models. 
*Risks* **5/4**, article 54.

Carvalho, E. (2017). Exploiting the use of recurrent neural networks for driver behavior profiling. *2017 International Joint Conference on Neural Networks*, 3016-3021.

Cather, D.A. (2020). Reconsidering insurance discrimination and adverse selection in an era of data analytics. *Geneva Papers on Risk and Insurance - Issues and Practice* **45**, 426–456. 

Cevolini, A., Esposito, E. (2020). From pool to profile: Social consequences of algorithmic prediction in insurance. *Big Data and Society* **7/2**.

<!-- Chollet, F., Allaire, J.J. (2018). *Deep Learning with R*. Manning Publication.  -->

Denuit, M., Guillen, M., Trufin, J. (2019). 
Multivariate credibility modelling for usage-based motor insurance pricing with behavioural data. *Annals of Actuarial Science* **13/2**, 378-399.

<!-- Esteves-Booth, A., Muneer, T., Kirby, H., Kubie, J., Hunter, J. (2001). -->
<!-- The measurement of vehicular driving cycle within the city of Edinburgh. -->
<!-- {\it Transportation Research Part D: Transport and Environment} {\bf 6/3}, 209-220. -->


<!-- Gao, G., Meng, S. and W\"uthrich, M. V. (2019). Claims frequency modeling using telematics car driving data.  -->
<!-- {\it Scandinavian Actuarial Journal} {\bf 2019/2}, 143-162. -->
 
<!-- Ferrario, A.,  Noll, A., W\"uthrich, M. V. (2018). Insights from inside neural networks. {\it SSRN}, abstract id: 3226852. -->
 
<!-- Gao, G.,  W\"uthrich, M. V.(2018). Feature extraction from telematics car driving heatmaps.  -->
<!-- {\it European Actuarial Journal} {\bf 8/2}, 383-406. -->
 
<!-- Gao, G., W\"uthrich, M. V. (2019). Convolutional neural network classification of telematics car driving data.  -->
<!-- {\it Risks} {\bf 7/1}, article 6. -->

Gao, G., Wang, H, Wüthrich, M.V. (2020). Boosting Poisson regression models with telematics car driving data. *SSRN* ID: 3596034.

Geyer, A., Kremslehner, D., Muermann, A. (2020). Asymmetric information in automobile insurance: Evidence from driving behavior. *Journal of Risk and Insurance* **87/4**, 969-995. 
  
<!-- Goodfellow, I., Bengio, Y., Courville, A. (2016). -->
<!-- *Deep Learning*. MIT Press. -->

Girma, A., Yan, X., Homaifar, A. (2019). Driver identification
based on vehicle telematics data using LSTM-recurrent neural network.
*2019 IEEE 31st International Conference on Tools with Artificial Intelligence*, 894-902.

Guillen, M., Nielsen, J.P., Pérez-Marín, A.M., Elpidorou, V. (2020).
Can automobile insurance telematics predict the risk of near-miss events?
*North American Actuarial Journal* **24/1**, 141-152. 
 
<!-- Henckaerts, R., Antonio, K., Clijsters, M., Verbelen, R. (2018). A data driven binning strategy for the construction of insurance tariff classes.  -->
<!-- *Scandinavian Actuarial Journal* **2018/8**, 681-705.  -->

<!-- Henckaerts, R., Côté, M.-P., Antonio, K., Verbelen, R. (2020). Boosting insights in insurance tariff plans with tree-based machine learning.  -->
<!-- *North American Actuarial Journal*. -->
  
Ho, S.-H., Wong, Y.-D., Chang, V. W.-C. (2014).
Developing Singapore driving cycle for passenger cars to estimate fuel consumption and vehicular emissions.
*Atmospheric Environment* **97**, 353-362.

Hu, X., Zhu, X., Ma, Y.-L., Chiu, Y.-C., Tang, Q. (2019).
Advancing usage-based insurance – a contextual driving risk modelling and analysis approach.
*IET Intelligent Transport Systems* **13/3**, 453-460.

Huang, Y., Meng, S. (2019). Automobile insurance classification ratemaking based on telematics driving data. 
*Decision Support Systems* **127**.

Hung, W.T., Tong, H.Y., Lee, C.P., Ha, K., Pao, L.Y. (2007).
Development of practical driving cycle construction methodology: a case study in Hong Kong.
*Transportation Research Part D: Transport and Environment*  **12/2**, 115-128.

Joubert, J. W., de Beer, D.,  de Koker, N. (2016).
Combining accelerometer data and contextual variables to evaluate the risk of driver behaviour.
*Transportation Research Part F: Traffic Psychology and Behaviour* **41/A**, 80-96.

Kamble, S.H., Mathew, T.V., Sharma, G.K. (2009).
Development of real-world driving cycle: case study of Pune, India.
*Transportation Research Part D: Transport and Environment*  **14/2**, 132-140.
  
Lemaire, J., Park, S.C., Wang, K. (2016). 
The use of annual mileage as a rating variable.
*ASTIN Bulletin* **46**, 39-69.

Ma, Y.-L., Zhu, X., Hu, X., Chiu, Y.-C. (2018). The use of context-sensitive insurance telematics data in auto insurance rate making.
*Transportation Research Part A: Policy and Practice*
**113**, 243-258.

Mahapatra, A. (2019). Privacy: A growing risk in the insurance industry. *Creative Components* 410.

Paefgen, J., Staake, T., Fleisch, E. (2014). 
Multivariate exposure modeling of accident risk: Insights from pay-as-you-drive insurance data. 
*Transportation Research Part A: Policy and Practice* **61**, 27-40.

Richman, R. (2020).
AI in actuarial science - a review of recent advances. 
*Annals of Actuarial Science*.

Romera, E., Bergasa, L.M., Arroyo, R. (2016). Need data for driver behaviour analysis? Presenting the public UAH-DriveSet. *2016 IEEE 19th International Conference on Intelligent Transportation Systems*, 387-392.

Savelonas, M. et al. (2020). Hybrid time-series representation for the classification of driving behaviour. *2020 15th International Workshop on Semantic and Social Media Adaptation and Personalization*, 1-6.

Verbelen, R., Antonio, K., Claeskens, G. (2018). Unraveling the predictive power of telematics data in car insurance pricing.
*Journal of the Royal Statistical Society: Series C (Applied Statistics)* **67**, 1275-1304.

Wahlström, J., Skog, I., Händel, P. (2017).
Smartphone-Based Vehicle Telematics:A Ten-Year Anniversary.
*IEEE Transactions on Intelligent Transportation Systems* **18/10**, 2802-2825.

Wahlström, J., Skog, I., Händel, P. (2015).
Detection of Dangerous Cornering inGNSS-Data-Driven Insurance Telematics.
*IEEE Transactions on Intelligent Transportation Systems* **16/6**, 3073-3083.

Wahlström, J., Skog, I.,  Nordström, R.L., Händel, P. (2018).
Fusion of OBD and GNSS Measurements of Speed. *IEEE Transactions on Instrumentation and Measurement* **67/7**, 1659-1667.
  
Weidner, W., Transchel, F.W.G.,  Weidner, R. (2016).
Classification of scale-sensitive telematic observables for riskindividual pricing.
*European Actuarial Journal* **6/1**, 3-24.

Weidner, W., Transchel, F.W.G.,  Weidner, R. (2017).
Telematic driving profile classification in car insurance pricing.
*Annals of Actuarial Science* **11/2**, 213-236.

<!-- Wiatowski, T., Bölcskei, H. (2018). -->
<!-- A mathematical theory of deep convolutional neural networks for feature extraction. -->
<!-- *IEEE Transactions on Information Theory* **64/3**, 1845-1866. -->


<!-- Wüthrich, M.V., Merz, M. (2019). Editorial: Yes, we CANN!  -->
<!-- *ASTIN Bulletin* **49/1**, 1-3.  -->

<!-- Yang, Y.,  Qian, W., Zou, H. (2018).  -->
<!-- Insurance premium prediction via gradient tree-boosted Tweedie compound Poisson models.  -->
<!-- *Journal of Business and Economic Statistics* **36/3**, 456-470. -->

<!-- \bibitem{Zhang1} -->
<!-- Zhang, W., Tanida, J., Itoh, K., Ichioka, Y. (1988). -->
<!-- Shift invariant pattern recognition neural network and its optical architecture. -->
<!-- {\it Proceedings of the Annual Conference of the Japan Society of Applied Physics}, 6p-M-14, 734. -->

<!-- \bibitem{Zhang2} -->
<!-- Zhang, W., Itoh, K., Tanida, J., Ichioka, Y. (1990). -->
<!-- Parallel distributed processing model with local space-invariant interconnections and its optical architecture. -->
<!-- {\it Applied Physics}  {\bf 29/32}, 4790-4797. -->

<!-- Zhu, X., Yuan, Y., Hu, X., Chiu, Y.-C., Ma, Y.-L. (2017). A Bayesian Network model for contextual versus non-contextual driving behavior assessment. -->
<!-- *Transportation Research Part C: Emerging Technologies* -->
<!-- **81**, 172-187. -->

















