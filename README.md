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
return result.isMinimumEntropyMet();


String timeToCrackOff = TimeEstimate.getTimeToCrackFormatted(result, "OFFLINE_BCRYPT_12");
String timeToCrackOn = TimeEstimate.getTimeToCrackFormatted(result, "ONLINE_THROTTLED");

if (result.isMinimumEntropyMet())
{
  StringBuilder successMessage = new StringBuilder();
  successMessage.append("Password has met the minimum strength requirements.");
  successMessage.append("<br>Time to crack - online: ").append(timeToCrackOn);
  successMessage.append("<br>Time to crack - offline: ").append(timeToCrackOff);

  setSuccessMessage(successMessage.toString());
  return true;
}
else 
{
  Feedback feedback = result.getFeedback();
  
  StringBuilder errorMessage = new StringBuilder();
  errorMessage.append("Password does not meet the minimum strength requirements.");
  errorMessage.append("<br>Time to crack - online: ").append(timeToCrackOn);
  errorMessage.append("<br>Time to crack - offline: ").append(timeToCrackOff);
  
  if(feedback != null)
  {
    if (feedback.getWarning() != null)
      errorMessage.append("<br>Warning: ").append(feedback.getWarning());
    for (String suggestion : feedback.getSuggestion())
    {
      errorMessage.append("<br>Suggestion: ").append(suggestion);
    }
  }
  
  setErrorMessage(errorMessage.toString());
  return false;
}

String pass1 = Generator.generatePassphrase("-", 5);
String pass2 = Generator.generatePassphrase(new Dictionary(...), "-", 5);

String pass = Generator.generateRandomPassword(Generator.CharacterTypes.ALPHANUMERIC, 15);
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


