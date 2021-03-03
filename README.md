# .NET-Core-MySql-Code-First

## How to use
***
Step # 1
```
Rename "ExperimentContext.cs" file as according
[Your DatabaseName]Context.cs
```

Step # 2
```
Inside "ExperimentContext.cs" rename ExperimentContext with [Your DatabaseName]Context
```

Step # 3
```
Register your model classes as according
public virtual DbSet<[Model Class Name]> [Coresponding Table Name] { get; set; }
```

Step # 4
```
Inside the main function in "Program.cs" update your constructor name and connection string
```

Step # 5
```
Run the program
```

## Update Connection String
***
Xampp localhost connection string is provided bellow
```
server=localhost;User Id=root;Database=test;Port=3306;
```
Update it like this
```
server=[Database Source];User Id=[Your User Id];Password=[Your Password];Database=[Your Database Name];Port=[Your Port];
```
***
***N.B:***
* This application will check is the database exists or not, if does, it shall create the tables, is it doesn't, it shall create the database by it self and then create the tables
* Models folder is an example which was tested functional with MySql in Xampp, thus it should work with any MySql server
***