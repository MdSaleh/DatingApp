
172.174.136.181/32,172.174.138.250/32,172.174.145.202/31,172.174.205.48/31,172.174.248.247/32,172.174.254.96/28,20.106.203.116/32,20.106.204.64/32,20.127.150.91/32,20.51.254.78/31,20.51.255.234/32,4.236.148.66/31,4.236.189.42/31,4.236.189.77/32,4.236.189.81/32,40.76.108.59/32,40.76.111.216/32,40.76.125.192/28,40.76.225.172/31,74.235.146.111/32,74.235.92.224/28




string connectionString = 
  @"mongodb://kafkabootcampdemo:6hEwV4G5HozYFQ4aCg7gDbLqHZAkCFIOZGzvwyNoSst9n0fPtXiX4thvzH9bzoM6lBdSsWZow0R0ACDbrQeyHA==@kafkabootcampdemo.mongo.cosmos.azure.com:10255/?ssl=true&retrywrites=false&replicaSet=globaldb&maxIdleTimeMS=120000&appName=@kafkabootcampdemo@";
MongoClientSettings settings = MongoClientSettings.FromUrl(
  new MongoUrl(connectionString)
);
settings.SslSettings = 
  new SslSettings() { EnabledSslProtocols = SslProtocols.Tls12 };
var mongoClient = new MongoClient(settings);
