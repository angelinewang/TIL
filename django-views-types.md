#### Function-Based Views
= More control over what happens inside the view
--> Compared to using *Class-Based Views

##### Code Example 
```
@api_view(['GET'])
  def tweets_list(request):
    tweets = Tweet.objects.all()
    serializer = TweetSerializer(tweets, many=True)
    return Response(serializer.data)
```
