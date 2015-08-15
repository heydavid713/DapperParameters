# DapperParameters
Facade of Dappers DynamicParameters class to facilitate unit testing.

Available on [NuGet](https://www.nuget.org/packages/DapperParameters/)

## Define in your dependency injection tool of choice
* Interface:       IDapperParameters
* Implementation:  DapperParameters

SimpleInjector example:

    container.Register<IDapperParameters, DapperParameters>(Lifestyle.Transient);

## Use in conjunction with DapperWrapper
When used with [DapperWrapper](https://github.com/half-ogre/dapper-wrapper), it is possible to unit test your data layer.

## Sample Unit Tests
Sample unit tests (and setups) are available in the source using Moq and SimpleInjector.