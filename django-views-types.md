#### Function-Based Views
##### Purpose
= More control over what happens inside the view
--> Compared to using *Class-Based Views*

##### Application
= Using Decorators

##### Code Example 
```
@api_view(['GET'])
  def tweets_list(request):
    tweets = Tweet.objects.all()
    serializer = TweetSerializer(tweets, many=True)
    return Response(serializer.data)
```

##### Documentation 
[Glossary of Methods Available](https://cdrf.co)
