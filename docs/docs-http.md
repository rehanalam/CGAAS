# 

Simple calculator API hosted on APIMATIC



## Server Configuration for Base URLs







# <a name="api_reference"></a>API Reference

* [Simple Calculator](#simple_calculator)

## <a name="simple_calculator"></a>![Endpoint Group: ](https://apidocs.io/img/class.png "Simple Calculator") Simple Calculator


### <a name="calculate"></a>![Endpoint: ](https://apidocs.io/img/method.png "Calculate") `GET` /{operation}

> Calculates the expression using the specified operation.



#### Path Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| operation | `Operation Type` |  ``` Required ```  | The operator to apply on the variables | `"SUM"` | 

#### Query Parameters
| Parameter | Type | Tags | Description | Example |
|-----------|------| ---- |-------------| ------- |
| x | `precision` |  ``` Required ```  | The LHS value | `221.119187365342` | 
| y | `precision` |  ``` Required ```  | The RHS value | `221.119187365342` | 

#### Responses
**200** 

Body (_precision_) 
```
221.119187365342
```


**412** 

> Could not compute the requested calculation
Body (_CouldNotCompute_) 
```
{
  "ServerMessage": "ServerMessage",
  "ServerCode": 221
}
```


[Back to API Reference](#api_reference)

