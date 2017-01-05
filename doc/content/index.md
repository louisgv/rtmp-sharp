---
weight: 10
title: API Reference
---

# Introduction

Document for the `rtmp-sharp` library.

# Initialization

> Initialize and return a context object

```csharp
static async Task InitializeClient()
	{
		try
		{
			var context = new SerializationContext();

			var options = new RtmpClient.Options()
			{
				// required parameters:
				Url = URL,
				Context = context
			};

			var writer = new AmfWriter(context);

			var client = await RtmpClient.ConnectAsync(options);

			//Console.WriteLine(client);

			Console.WriteLine("CONNECTED!");
		}
		catch (Exception ex)
		{
			Console.WriteLine("EXCEPTION...");
			Console.WriteLine(ex.Message);
		}
	}
```

Error:

Operation not supported: Something wrong with the socket.io implementation?


# Write

> Initialize and return a context object

```csharp



```
