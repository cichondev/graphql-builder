# Graphql Builder

With this package you can build GraphQL queries using OOP, with a fluent interface.

## Example

`
<?php 

$query = GraphQLBuilder\Query::create('dogs')
            ->setParameter('breed', 'viralata')
            ->setFields(['id', 'age', 'size', 'color'])
            ->toString();
echo $query;
?>

Output: "uery dogs { dogs(breed: "viralata") { id, age, size, color } }"
`
