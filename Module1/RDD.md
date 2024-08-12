# What are RDDs?

Resilient Distributed Datasets (RDDs) are a fundamental data structure in the Apache Spark framework, designed to facilitate distributed data processing across clusters. RDDs serve as the foundational building blocks for Spark applications, enabling fault-tolerant, parallelized data processing in a distributed computing environment.

Key characteristics of RDDs include:

1. **Resilience:** RDDs are "resilient" because they can recover from node failures. Through lineage information, Spark can recreate lost data partitions by recomputing them from the original data and transformations.
2. **Distributed:** RDDs are distributed across multiple nodes in a Spark cluster, allowing for parallel processing of data. Each RDD is divided into partitions, with each partition residing on a separate node.
3. **Immutable:** RDDs are immutable, meaning their content cannot be changed once created. Instead, transformations applied to RDDs produce new RDDs, preserving data integrity.
4. **In-Memory Processing:** RDDs are stored in memory, enabling faster data access and computation compared to traditional disk-based storage. This in-memory processing contributes to Spark's speed advantage.
5. **Transformation and Action Operations:** RDDs support two types of operations: transformations (e.g., map, filter, reduceByKey), which create new RDDs from existing ones, and actions (e.g., count, collect, saveAsTextFile), which trigger computations and return results.
6. **Data Partitioning:** RDDs allow users to control data partitioning, which can optimize data locality and enhance processing efficiency.


# Getting Started: Creating RDD's with PySpark

Before you embark on the following coding exercise, let's take a moment to recap the foundational concepts you'll be working with. In this exercise, you'll be using PySpark, a Python library for Apache Spark, which is a powerful framework for distributed data processing. Spark allows you to efficiently process and analyze large datasets in a distributed and parallelized manner.

You'll start by launching a PySpark interactive session using the pyspark command. This session provides you with access to a Spark session object named spark, which acts as an entry point to interact with Spark's functionality. Additionally, you'll have access to a Spark context object named sc, which is the core interface for creating and manipulating resilient distributed datasets (RDDs), Spark's fundamental data abstraction.

Throughout the exercise, you'll work with a list of numbers and transform them using RDDs. An RDD is a distributed collection of data that can be processed in parallel. You'll create an RDD named 'rdd' from the list of numbers using the Spark context. You'll perform various operations on this RDD, such as counting the number of items, finding the maximum and minimum values, and calculating the mean.

Later in the exercise, you'll explore the concept of transformations and actions. Transformations create a new RDD from an existing one, while actions compute a result and return it to the driver program or write it to an external storage system.

You'll apply transformations like mapping and filtering to the original RDD, creating a new RDD named 'rdd2' with squared values and another RDD named 'even' with only even values.

By the end of this exercise, you'll have gained hands-on experience with PySpark's basic operations, including creating RDDs, performing transformations and actions, and collecting data from RDDs. This foundational knowledge will set the stage for more advanced data processing and analysis tasks using Spark. Let's dive in and start exploring the capabilities of PySpark!
