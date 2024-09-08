

# Administering an AlloyDB Database || [GSP1086](https://www.cloudskillsboost.google/focuses/50121?parent=catalog) ||

# # Like, comment, share & Don't forget to subscribe [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

---


### 🔗 GO TO - [``AlloyDB``](https://console.cloud.google.com/alloydb/clusters?referrer=search&project=)

### 🔗 GO TO - [``VM Instance``](https://console.cloud.google.com/compute/instances?referrer=search&project=)



PASTE THESE FOLLOWING COMMANDS IN `SSH` WINDOW 

```bash
export ALLOYDB=
```

```
echo $ALLOYDB  > alloydbip.txt
```

```bash
psql -h $ALLOYDB -U postgres 
```

- user's password
```
Change3Me
```

```bash
\c postgres
```

```bash
CREATE EXTENSION IF NOT EXISTS PGAUDIT;
```

```bash
select extname, extversion from pg_extension where extname = 'pgaudit';
```



 **Launch Cloud Shell:**  
 
-  [``Cloud Shell``](https://console.cloud.google.com/home/dashboard?project=&pli=1&cloudshell=true)


```bash
export REGION=
```

```bash
gcloud alloydb instances create lab-instance-rp1 \
  --cluster=lab-cluster \
  --region=$REGION \
  --instance-type=READ_POOL \
  --cpu-count=2 \
  --read-pool-node-count=2
```

 **Launch Another Cloud Shell By Clicking on +**  


```bash
export REGION=
```

```bash
gcloud beta alloydb backups create lab-backup --region=$REGION  --cluster=lab-cluster
```

---

# Congratulations ..!!🎉  You completed the lab shortly..😃💯

# *Well done..!* 👏

# Thank you for visiting.... :) 🗯️

# [Qwiklab_Explorers_ts](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)
