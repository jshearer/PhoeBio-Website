![Alt text](https://g.gravizo.com/source/svg/custom_mark12?https%3A%2F%2Fraw.githubusercontent.com%jshearer%2FPhoeBio-Website%2Fmaster%2domain_model.md)
<details> 
<summary></summary>
custom_mark12
@startuml domain model

entity Ontology {
  Process
  Function
  Component
  --
  **Example namespaces:**
  * Molecular function
  * Cellular component
  * Biological process
  
  Note: One GO Term is \ncontained within one namespace
}

entity "GO Term" as Term {
  GO Terms are a DAG so
  they may have many
  parents and many children
}

entity "Gene Product" as GeneProduct {

}

entity Annotation {
  description
  reference
  methods
  --
  # evidence code enum  
    Interresting terms:
    **ND** - No Bio. Data Available

    EXP, IDA, IPI ...
}

entity Gene {

}

entity "Gene Function" as GeneFunction {

}

entity "GO Slim" as Slim {

}

entity "Annotation Dataset" as ADS {

}

entity "Experimental Evidence" as Evidence{
  
}

entity Aspect {

}

Note "Identifies a Gene with a \npiece of research, a function, \na location, etc" as N1

Ontology<-down-Term: Supports
Annotation-down->Term: "Associates with \nGene Product"
GeneProduct "1" -right-> "0 or more" Term: Is Annotated To
Gene-right->GeneProduct: Encodes
Annotation-->GeneProduct: "Associates with \nGO Term"
GeneProduct "1" --> "1 or more" GeneFunction: Enables
Slim-->Term: Chosen subset of
Slim-left->Annotation: Bins on (filter,query, etc)
Annotation-up->ADS: Recorded in
Evidence-->Annotation: Backs up
N1<..Annotation
N1..>Gene
' Term-->Term: Related to
Aspect<-right-Term: "Is categorized by\none ane only one"

' Ontology<-down-Term: Supports
' Annotation-down->Term: "Associates with \nGene Product""
' Term "0 or more" <-left- "1" GeneProduct: Is Annotated To
' Gene-right->GeneProduct: Encodes
' Annotation-->GeneProduct: "Associates with \nGO Term"
' GeneProduct "1" --> "1 or more" GeneFunction: Enables
' Slim-->Term: Chosen subset of
' Slim-left->Annotation: Bins on (filter,query, etc)
' Annotation-up->ADS: Recorded in
' Evidence-->Annotation: Backs up
' N1<..Annotation
' N1..>Gene
' ' Term-->Term: Related to
' Aspect<-right-Term: "Is categorized by\none ane only one"

@enduml
custom_mark12
</details>
