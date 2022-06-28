#DapperParameters.Core

This is a fork of the original [DapperParameters](https://github.com/IntertechInc/DapperParameters) project that is compiled to .NET Standard 2.0 instead of the original .NET Framework 4.0.

The Nuget feed for this project is found [here](https://www.nuget.org/packages/DapperParameters.Core/)

If there's any issues please open a new Issue here on GitHub.

The details of the original project is found below.

# DapperParameters
Facade of Dappers DynamicParameters class to facilitate unit testing.

Available on [NuGet](https://www.nuget.org/packages/DapperParameters/)

Blog post [here](http://www.intertech.com/Blog/unit-test-dapper-with-dapperparameters/)

## Define in your dependency injection tool of choice
* Interface:       IDapperParameters
* Implementation:  DapperParameters

SimpleInjector example:

    container.Register<IDapperParameters, DapperParameters>(Lifestyle.Transient);

## Use in conjunction with DapperWrapper
When used with [DapperWrapper](https://github.com/half-ogre/dapper-wrapper), it is possible to unit test your data layer.

## Sample Unit Tests
Sample unit tests (and setups) are available in the source using Moq and SimpleInjector.
