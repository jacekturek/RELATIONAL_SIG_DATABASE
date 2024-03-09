# Do some relational math - queries

Relations = tables have attributes:
SELECT DISTINCT will show RANKINGS (IN ME) in the database:

SELECT DISTINCT [RANKING IN ME]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[RANKINGS]
  
![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/c2a3e9de-c2b3-4aca-9c94-1bb6b5f9e1f8)

> ℹ️ The number of attributes (cardinality) and number of rows (degree) is an obvious feature of the relational database.

> Here these two numbers prove to be enough to achieve the understanding of SEO data in social media pages.

# Selection

Select with selection condition, here an example
SELECT
> ✍️table signal_perc
> 
> ✍️selction condition who = 'GW'

This command is from SQL server programm, showing the generated command:

SELECT TOP (1000) [where_from]
      ,[perc]
      ,[signal_name]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[SIGNALS_PERC]
  WHERE where_from = 'GW'
  
![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/39f03a50-65cd-44f8-b5cb-2a76e9b2a36e)

Thinking about selection condition:
> it can be any other comparison e.g. "<" etc.
> 
> 🎓 obviously there is no signal < 2 (coming from the selected source)

Including the logical operators (OR, AND):

SELECT [SIGNAL]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[ENGAGEMENT]
  WHERE [ENAGEMENT] = 'IDENTITY' OR [SIGNAL] = '2'

![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/745194cc-3fd5-417f-a9a1-436f67269fa6)

Only to mention:
> nested select operator (in theory):
> 
> S condition (S conditon (TABLE)) - unary operation
> 
> or the number of rows from select, which is: 0 < select < number of rows

# Projection

> some attributes from a table, which can show some important conclusions:

![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/faf00477-68be-4cdc-a74d-1aa7af3809c5)

SELECT TOP (1000) [WHAT]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[EAT ALGORITHM]

![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/4f3a89dc-5b06-4471-bfa4-ecc1cd3259b7)

# Union (SQL)

SELECT TOP (1000) [signal_name]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[SIGNALS_PERC]
  
  UNION 

  SELECT TOP (1000) [SIGNAL]
  FROM [SEO_SIG_IN_SOC_MEDIA].[dbo].[ENGAGEMENT]

![image](https://github.com/jacekturek/RELATIONAL_SIG_DATABASE/assets/62720909/fb790d89-954b-48d1-a019-a283fcfe42df)

> ENGAGEMENT is saying what is the purpose of the signal
> 
> PERC how much i can see it on my page

Interesting queries.

# Intersection and minus

> In short:

Intersection of the above relations is the same as the union (the disctinct signals are the same).

Minus will in obvious way return 0 (empty).

