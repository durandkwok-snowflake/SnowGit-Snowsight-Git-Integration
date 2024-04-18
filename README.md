# SnowGit-Setup
## With SnowGit read-only in Snowsight user can now:

*Connect to an existing git repository via the Create object → Git Repository flow in the UI

*See all their branches, tags and folders and files inside their repository

*Fetch the latest version of their files via the UI

*Execute immediate SQL files directly from the repo (after seeing a code-preview)

*Copy the path to a repo file to be used in a script or app or notebook

*Copy the code from a SQL-script template into a worksheet to modify and run it

*Download a file from the repo to use it locally
### Create API INTEGRATION

<img width="1235" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/3f63db31-5e8f-476b-bede-c9cc596c7758">

```SQL
CREATE OR REPLACE API INTEGRATION git_api_integration_scaling_test
  API_PROVIDER = git_https_api
  API_ALLOWED_PREFIXES = ('https://github.com/durandkwok-snowflake/DK_Snowflake_Scaling_Compute_Demo.git')
  --ALLOWED_AUTHENTICATION_SECRETS = (git_secret)
  ENABLED = TRUE;
```
### Select a Database and Schema to Create Git Repository Integration
<img width="275" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/def78c08-3756-4fc6-adc1-dcd205e9298a">

<img width="1147" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/1a02b83d-9372-4002-85c9-1faeaebf6892">

<img width="183" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/2f45b58a-cd60-4b88-94bb-52a34be05896">

<img width="572" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/4391eff9-720f-46c8-8934-8d9b57821a0b">


<img width="502" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/0a603ec3-2e49-4b8e-bed9-62c292d83239">

### Enter Repository Name
<img width="494" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/5611293a-83cb-4576-a630-deeb91ce8bca">

### Enter Origin
#### Fetch the URL from the Github you want to integrate with

<img width="493" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/9ed4517a-8c58-4698-98d8-5eed3a410971">

#### and populate the Origin field from Setup

<img width="480" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/6c72bf44-626d-4ec9-81bf-414962814307">

#### Select the API Integration from the drop down list

<img width="499" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/41f592fc-c97b-420c-9490-56fb3566a962">

#### Select Enable Authentication if your repository is private (Note: My repository is public therefore I did not enable authentication)

<img width="500" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/b5e7e46b-d104-421b-a4b5-92c33f3c18f2">

### Select Create to proceed

<img width="144" alt="image" src="https://github.com/durandkwok-snowflake/SnowGit-Read_Only_UI/assets/109616231/54926133-3459-4306-84e9-f01f1b30d816">





