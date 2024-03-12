It is a repository for the dataset based on Spring Cloud style microservice systems.

This dataset contains 1195 data points.

## The attributes of feature data.

| num  | attribute          | type                                      | annotation                                                   |
| ---- | ------------------ | ----------------------------------------- | ------------------------------------------------------------ |
| 1    | sysName            | String                                    | microservice system name                                     |
| 2    | serviceName        | String                                    | name of microservice in the system                           |
| 3    | releases           | String                                    | release tag of the current system                            |
| 4    | codeSize           | Integer                                   | the effective lines of source code                           |
| 5    | entityNum          | Integer                                   | the number of entity classes                                 |
| 6    | entityAttributeNum | Integer                                   | the number of controller classes                             |
| 7    | aveEntityAttribute | Double                                    | value of dividing entityAttributeNum by entityNum            |
| 8    | controllerNum      | Integer                                   | the number of controller classes                             |
| 9    | interfaceNum       | Integer                                   | the number of interface classes                              |
| 10   | abstractClassNum   | Integer                                   | the number of abstract class                                 |
| 11   | serviceClassNum    | Integer                                   | the number of service implementation class                   |
| 12   | dtoObjectNum       | Integer                                   | the number of data transfer object classes                   |
| 13   | APINum             | Integer                                   | the number of APIs exposed                                   |
| 14   | maxParaNum         | Integer                                   | The maximum value of the parameter list size for each API    |
| 15   | APIVersionNum      | Integer                                   | the number of API versions                                   |
| 16   | APIVersionSet      | String                                    | the set of versions                                          |
| 17   | serviceImplCall    | String(key-value. **service-func:times**) | The keys correspond to the methods of service implementation classes invoked in the controller classes within the microservice. The values in the collection represent the count of internal invocations for each method. |
| 18   | serviceImplCallNum | Integer                                   | the total number of invocations from controller to service implementation |
| 19   | serviceCall        | String(key-value. **service:times**)      | *Map <serviceA, <ServiceB,times>>*, where ServiceA acts as the primary key, ServiceB serves as the nested key, and the associated value, times, denotes the frequency of ServiceA invoking ServiceB. |
| 20   | maxServiceCall     | Integer                                   | The maximum number of times the current microservice invokes other microservices. |
| 21   | serviceCallCate    | Integer                                   | a.  The number of distinct microservices invoked by the current microservice. |
| 22   | serviceCallPer     | double                                    | The percentage of distinct microservices invoked by the current microservice out of the total number of microservices in the system. |
| 23   | serviceCalled      | String(key-value. **service:times**)      | *Map <serviceA, <ServiceB,times>>*, where ServiceA acts as the primary key, ServiceB serves as the nested key, and the associated value, times, denotes the frequency of ServiceA being invoked by ServiceB. |
| 24   | maxServiceCalled   | Integer                                   | The maximum number of times the current microservice is called by other microservices. |
| 25   | serviceCalledCate  | Integer                                   | The number of distinct microservices that invoke the current microservice. |
| 26   | serviceCalledPer   | double                                    | The percentage of distinct microservices that invoke the current microservice out of the total number of microservices in the system. |

The data is pure without annotate.

## to download

git clone https://github.com/yang66-hash/Spring-Cloud-Microservice-Dataset.git
