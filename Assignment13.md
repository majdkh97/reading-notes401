# Read13

## Related data in Spring
### One-to-One Relationship 
- A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.

- define two entity classes Library and Address having a one-to-one relationship, using the @OneToOne annotation. The association is owned by the Library end of the association
- We must be careful to have different names for each association resource. 
- Otherwise, we will encounter a JsonMappingException with the message: “Detected multiple association links with same relation type! Disambiguate association”.

### One-to-Many Relationship
- A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.

### Many-to-Many Relationship
- A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.

## Integration Testing
**Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.**