# FAIRification Process
[https://www.go-fair.org/fair-principles/fairification-process/
]()  

Most of the requirements for findability and accessibility can be achieved at the metadata level. Interoperability and reuse require more efforts at the data level. 


**Retrieve non-FAIR data**: gain access to the data to be FAIRified.

**Analyse the retrieved data**: inspect the content of the data: Which concepts are represented? 
What is the structure of the data? What are the relations between the data elements? Different data distributions require different methods for identification and analysis. For instance, if the dataset is in a relational database, the relational schema provides information about the dataset structure, the types involved (the field names), cardinality, etc.

**Database model**  
Define the semantic model: define a ‘semantic model’ for the dataset, which describes the meaning of entities and relations in the dataset accurately, unambiguously, and in a computer-actionable way. Depending on the dataset, defining a proper semantic model may require a significant effort, even for experienced data modellers. A good semantic model should represent a consensus view in a particular domain, for a particular purpose. Therefore, it is good practice to search for existing models. Semantic models often contain multiple terms from existing ontologies and vocabularies. A vocabulary is a computer-readable file that captures terms, their URIs, and descriptions. An ontology can be roughly described as a vocabulary with hierarchies, meaningful relations among concepts, and their constraints. These conceptual models allow us to classify our data models and data items using the provided terms, concepts, and conceptual structures.

**Make data linkable**: The non-FAIR data can be transformed into linkable data by applying the semantic model defined in step 3. Currently, this is done using Semantic Web and Linked Data technologies. This step promotes interoperability and reuse, facilitating the integration of the data with other types of data and systems. However, the user should evaluate the feasibility of this step for the given data. It is a sensible thing to do for many types of data (e.g., structured data), but it may not be relevant for other types (e.g., the pixels or audio elements in images, audio data, and videos). Of course, the annotations about the images, audio, and video (e.g., data about identified regions of images, or about parts of an audio file) could very well be made linkable.

**Assign license**: Although license information is part of the metadata, we have incorporated the license assignment as a separate step in the FAIRification process to highlight its importance. The absence of an explicit license may prevent others to reuse data, even if the data is intended to be open access.

The conditions under which the data can be used should be clear to machines and humans.
Examples
Commonly used licenses like MIT or Creative Commons can be linked to your data. Methods for marking up this metadata are provided by the DTL FAIRifier.
Links to Resources
https://wiki.creativecommons.org/wiki/License_RDF


Define metadata for the dataset: As explained by many of the FAIR principles, proper and rich metadata support all aspects of FAIR. (Read the GO FAIR recommendation for metadata.)

Deploy FAIR data resource: deploy or publish the FAIRified data, together with relevant metadata and a license, so that the metadata can be indexed by search engines and the data can be accessed, even if authentication and authorisation are required.



**FAIR Requirements**  
* Data and Metadata (RDF -Resource Description Framework )  
* Modelo de la base de datos  
* Ontologies and vocabularies  
* Semantic Web and Linked Data technologies  
* License  


Nanomaterials

The NMDataParser tool can be used as a component of a data import workflow or as a standalone application to convert data from non-FAIR Excel files into different structured semantic formats *(RDF, JSON–LD, JSON, ISA–JSON)*.


Thus, the approach taken early on by eNanoMapper was to develop a tool to help in converting the existing variety of spreadsheets into a common semantic data model, incorporate annotation with ontology terms, and steer the spreadsheet layout design towards harmonization, while retaining the user friendliness and features deemed important by the labs.

as well as many customized methods for accessing the data through a REST API via external tools like Jupyter notebooks and the KNIME analytics platform.


Interactive documentation of the API in OpenAPI v3 format is available at https://api.ideaconsult.net/ for each of the imported datasets (Figure 10).

Multiple data export formats are supported by the eNanoMapper database instances (both in
the web user interface and the API), including the semantic formats (RDF, JSON–LD).
eNanoMapper database export: serialization as JSON, RDF, and Excel/CSV.

Availability
The Nanosafety search interface is available at https://search.data.enanomapper.net/.
The eNanoMapper database instances and the Nanosafety search interface are hosted and maintained by Ideaconsult Ltd. The eNanoMapper database code is open source and available at http://ambit.sf.net.
We provide Docker images and docker-compose configurations to allow convenient and quick set up of the required stack of software components. At present, the components included in the docker-compose setups are the Ambit platform and the eNanoMapper database, which also may be pre-populated with

Metadata that is easily findable, accessible and interoperable makes reuse of the experimental data feasible in a more practical manner for solving serious scientific problems, data gap filling, read across applications, QSAR/QSPR modelling and in supplying tools for other needs of the science, industry and regulators in the context of Safe-by-design
NMs. Rich metadata layers, which are easily understood on a conceptual level and to be used practically, are one of the major milestones of the FAIRification process.

