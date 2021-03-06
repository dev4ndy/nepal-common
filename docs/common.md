<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [@al/common](./common.md)

## common package

## Classes

|  Class | Description |
|  --- | --- |
|  [AlAPIServerError](./common.alapiservererror.md) | This error should be used when an HTTP 5xx response (or other general error) is received from an internal API. |
|  [AlBadRequestError](./common.albadrequesterror.md) | Used to indicate an invalid request to a service or API. |
|  [AlBaseError](./common.albaseerror.md) | A base error class used only to provide consistent prototype chaining. |
|  [AlBehaviorPromise](./common.albehaviorpromise.md) | AlBehaviorPromise is a simple extension of Promise that replicates the functionality provided by RxJS's BehaviorSubject. Promises already provide multicasting functionality, but it can be deucedly inconvenient to provide an inline executor, and rather obtuse to change the resolved value.<!-- -->This class exposes the basic surface area of a Promise -- it is <code>then</code>able -- but allows the resolved value to change if necessary. |
|  [AlCabinet](./common.alcabinet.md) | AlCabinet provides a simple, generic interface for caching arbitrary data. It supports optional serialization to localStorage and sessionStorage, where available, but will gracefully fallback to in-memory-cache mode in their absence. |
|  [AlGlobalizer](./common.alglobalizer.md) | AlGlobalizer is a simple tool for exposing encapsulated code selectively in global scope, and for ensuring that singleton instances are, in fact, singletons. |
|  [AlLocation](./common.allocation.md) | AlLocationType is an enumeration of different location types, each corresponding to a specific application. Each type is presumed to have a single unique instance inside a given environment and residency. |
|  [AlLocatorMatrix](./common.allocatormatrix.md) | This class accepts a list of location descriptors, an acting URL, and an optional context specification, and provides the ability to calculate environment- and residency- specific target URLs. |
|  [AlResponseValidationError](./common.alresponsevalidationerror.md) | The AlResponseValidationError is intended to alert of unexpected responses from an internal API. These responses need to be identified separately from other errors so that the relevant system health checks or communication with an appropriate backend team can be organized in response. Please note that this should NOT be used to handler general server-side failures; please see AlAPIServerError for that error condition. |
|  [AlRoute](./common.alroute.md) | An AlRoute is an instantiated route definition, attached to a routing host, and capable of actually calculating target URLs based on context and handling navigation events. |
|  [AlStopwatch](./common.alstopwatch.md) | AlStopwatch is an attempt to encapsulate a few basic timer-related use cases into a simple interface. Most uses cases can be handled by one of the three static methods: <code>Stopwatch.later</code> - creates a Stopwatch instance that won't be executed until someone calls its <code>now</code> or <code>again</code> methods. <code>Stopwatch.once</code> - creates a Stopwatch instance that executes once after a specified delay, defaulting to 0. <code>Stopwatch.repeatedly</code> - creates a Stopwatch instance that executes repeatedly at a given interval until its <code>cancel</code> method is called. |
|  [AlSubscriptionGroup](./common.alsubscriptiongroup.md) | This is a simple utility to manage a list of subscriptions, which may be AlTriggerSubscriptions or RxJS subscriptions. It exposes a method <code>manage</code> to add new subscriptions, and a method <code>cancelAll</code> to unsubscribe from all subscriptions. That is all it does. |
|  [AlTriggeredEvent](./common.altriggeredevent.md) | Represents a typed event. |
|  [AlTriggerStream](./common.altriggerstream.md) | Represents a series of triggered events. |
|  [AlTriggerSubscription](./common.altriggersubscription.md) | Represents a subscription to a stream of triggered events. |
|  [AlUnauthenticatedRequestError](./common.alunauthenticatedrequesterror.md) | Used to indicate that the current actor is not authenticated. |
|  [AlUnauthorizedRequestError](./common.alunauthorizedrequesterror.md) | Used to indicate that the current actor is not authorized to perform a given action. |

## Functions

|  Function | Description |
|  --- | --- |
|  [AlTrigger(eventTypeName)](./common.altrigger.md) | Annotation for trigger type classes. Prevents unique event type names from being lost during minification/uglification. |

## Interfaces

|  Interface | Description |
|  --- | --- |
|  [AlLocationContext](./common.allocationcontext.md) | AlLocationContext defines the context in which a specific location or set of locations may exist. - environment - development, integration, production? - residency - US or EMEA (or default)? - insightLocationId - insight-us-virginia, insight-eu-ireland, defender-us-ashburn, defender-us-denver, defender-uk-newport - accessible - a list of accessible insight location IDs |
|  [AlLocationDescriptor](./common.allocationdescriptor.md) | Describes a single instance of a location type (AlLocation). |
|  [AlNavigationSchema](./common.alnavigationschema.md) | This is a top-level interface for the structure of a schema document, which is a set of compiled menus and behavioral rules. |
|  [AlRouteAction](./common.alrouteaction.md) | The action associated with a route. These are only the most common properties. |
|  [AlRouteCondition](./common.alroutecondition.md) | Conditional expressions |
|  [AlRouteDefinition](./common.alroutedefinition.md) | This is an abstract definition for a single menu item or menu container. |
|  [AlRoutingHost](./common.alroutinghost.md) | Any navigation host must provide these basic functions |

## Variables

|  Variable | Description |
|  --- | --- |
|  [AlInsightLocations](./common.alinsightlocations.md) | A dictionary of insight locations (as reported by AIMS and the locations service). |
|  [AlLocationDictionary](./common.allocationdictionary.md) | A dictionary of public Alert Logic resource locations, subkeyed by residency and environment. |
|  [AlLocatorService](./common.allocatorservice.md) | Global singleton instance of [AlLocatorMatrix](./common.allocatormatrix.md)<!-- -->. |

## Type Aliases

|  Type Alias | Description |
|  --- | --- |
|  [AlTriggeredEventCallback](./common.altriggeredeventcallback.md) | Callback type for triggered events. |

