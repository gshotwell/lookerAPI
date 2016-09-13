 
 To install run: 
 ```
 devtools::install_github( REPO,
 auth_token = PAT)
 
 ```
 Making sure to sub in your personal access token generated from in https://github.com/settings/tokens
 
 To access the looker API you need to get API3 credentials. To do this open the looker GUI and go to Admin > Users then select the user and click "New API 3 Key". These keys should be saved in your .Renviron file and never stored in code. For instructions on how to do this see [this guide](https://github.com/hadley/httr/blob/master/vignettes/api-packages.Rmd#appendix-storing-api-authentication-keystokens). It's best to name these keys `LOOKER_API_3_CLIENT` and `LOOKER_API_3_SECRET` in the .Renviron file, but you can name them whatever you like. 


To use this package, first build the look in looker and then save it. The id of the look is displayed as the last number in the URL after `look_id=`. To fetch the results of this look call `run_look(look_id)`, this will log you in  
 
