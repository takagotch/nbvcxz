### nbvcxz
---
https://github.com/GoSimpleLLC/nbvcxz

```java
Nbvcxz  nbvcxz = new Nbvcxz();

Configuration configuration = new ConfigurationBuilder()
  .setLocale(Locale.forLanguageTag("Tag"))
  .createConfiguration();
  
Nbvcxz nbvcxz = new Nbvcxz(configuration);

List<Directory> directoryList = ConfigurationBuilder.getDefaultDictionaries();
dictionaryList.add(new DictionaryBuilder()
  .setDictionaryName("exclude")
  .setExclustion(true)
  .addWord(user.getFirstName(), 0)
  .addWord(user.getLastName(), 0)
  .addWord(user.getEmail(), 0)
  .createDictionary());
  
Nbvcxz nbvcxz = new Nbvcxz(configuration);

Result result = nbvcxz.estimate(password);




```

```sh
apt-get install git
apt-get install openjdk-8-jdk
apt-get install maven
git clone https://github.com/GoSimpleLLC/nbvcxz.git
cd nbvcxz
mvn package

```

```
```


