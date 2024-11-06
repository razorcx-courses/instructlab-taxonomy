







Tekla.Structures.Model Namespace















Tekla Open API Reference for Tekla Structures 2023




|  | Tekla.Structures.Model Namespace |
| --- | --- |


\[This is preliminary documentation and is
 subject to change.]


The Tekla.Structures.Model namespace includes the functionality to insert, select, modify
 or delete objects inside a Tekla Structures model. The namespace also includes possibilites to query
 different kind of data from the current model instance, such as information about the currently selected
 objects. The namespace offers the functionality through .NET remoting and the COM interface.
Classes



|  | Class | Description |
| --- | --- | --- |
|  | [Assembly](05895e96-9746-fce3-380b-7892400ca1b8.htm) | The Assembly class defines a single manufacturing unit: objects that are bolted or welded  together in the workshop.  An assembly has a main part and secondary assemblables attached to it. The number of secondaries  is limited to 2048\.  Hierarchical assemblies can also have subassemblies attached to them and they can have a parent  assembly instance. |
|  | [BaseComponent](3f5c4af6-b37c-5f30-9ce4-ea5f2bf028fe.htm) | The BaseComponent class is an abstract base class that represents generic components. The  generic components  derived from the base component are the component, the connection, the detail and the seam. |
|  | [BasePoint](5c1b45f5-9a0b-cd81-ec51-dd4e21ff20ce.htm) | The BasePoint class provides base point related functionalities. Base points can be retrieved  using  ProjectInfo class. |
|  | [BaseRebarGroup](2102980d-739e-ab9a-1311-c4c494dc6d42.htm) | The BaseRebarGroup class is an abstract base class that represents reinforcing bar group  classes.  The reinforcing bar groups derived from the base group are the rebar group, the circled rebar  group  and the curved rebar group. |
|  | [BaseRebarModifier](f2d8320f-58b5-3669-bde6-a6bdf71d6062.htm) | Represents a modifier that can modify the characteristics of [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) reinforcing bars that pass  through it. |
|  | [BaseWeld](173a061a-4957-ea9e-e87e-3949c3c7a653.htm) | The BaseWeld abstract class defines a weld between two model objects. |
|  | [Beam](8621e658-a496-c1b9-49d0-4076c20779f7.htm) | The Beam class represents a single beam in the model.  A beam has a single start and end point. |
|  | [BendSurface](4b8c0f69-2f54-749d-5dcc-753991f7481f.htm) | The BendSurface class defines a surface contour that can be used as a bend between two plates |
|  | [BendSurfaceNode](587d9a1d-e196-e65c-eaf5-130c137c8b60.htm) | The BendSurfaceNode class represents a bend surface geometry tree node. |
|  | [BentPlate](a75e430c-a12d-1753-65b0-f93472716a4a.htm) | A class for the bent plate |
|  | [BentPlateGeometrySolver](6868795d-e6b6-4c94-a705-5e4972e535c9.htm) | BentPlateGeometrySolver is a solver class to handle ConnectiveGeometry modification related  computations. |
|  | [BoltArray](caa3aee3-d7ae-6c96-bce9-eaab89a1cad5.htm) | The BoltArray class defines a bolt group with an array shape. |
|  | [BoltCircle](344a2e05-14de-2b76-e846-28e68b0c68ae.htm) | The BoltCircle class defines a bolt group with a circle shape. |
|  | [BoltGroup](3647beae-3e71-72e2-03ee-df67381da5db.htm) | The BoltGroup class is an abstract base class for all bolt shapes, such as array, circle and XY  list.  See the Tekla Structures help file for further information about the attributes. |
|  | [BoltHoleAttributes](422ddb23-4ec9-3422-853d-aac6c307683d.htm) | The bolt hole attributes. |
|  | [BoltXYList](46d4ad9b-0db9-51b1-caa4-74a439cd54fc.htm) | The BoltXYList class defines a bolt group with an XY list shape. The bolt group is the most  generic one  of the bolt groups. |
|  | [Boolean](49be33d1-5e49-b9cf-a30f-6292868e03a5.htm) | The Boolean class is an abstract base class for boolean operations such as a part cut, an add, a  fitting or  a cut plane. |
|  | [BooleanPart](2fbf5949-ba94-3e0d-a738-1ed7ba1bec1d.htm) | The BooleanPart class represents a part cut or an add. This means that a model object is, for  example,  cut with a part instance to create a void to the father part. Typically the operative part is  deleted after  the boolean cut operation. In case of boolean add, operative part is deleted automatically. |
|  | [Brep](77e7ce8e-76cd-c1d8-1814-1b02750fa9bc.htm) | The Brep class represents a single brep in the model.  A brep has a single start and end point. |
|  | [Chamfer](3064a4cf-a8fc-6b76-b9e1-01173be467df.htm) | The Chamfer class defines how the corners of a polybeam or a contour plate are rounded. |
|  | [ChangeData](71408208-1126-6f3d-f4a1-8e524f7875da.htm) | The ChangeData class presents information about the detected change of the modelobject in the  model. It is instantiated inside the connected method. |
|  | [CircleRebarGroup](8b1ad479-c856-307c-b1c3-87b6ad423bec.htm) | The CircleRebarGroup class represents a group of reinforcing bars which have a circular shape. |
|  | [ClashCheckData](2e113655-9825-9801-b873-2dc75b1549f1.htm) | The ClashCheckData class presents information about the detected clash. It is instantiated  inside the onClashDetected method.  The objects store the identifiers and type of the clash to be passed on to event subscribers. |
|  | [ClashCheckHandler](788112d7-7e99-4d1c-c631-4c1a23366696.htm) | The ClashCheckHandler class contains clash check methods. |
|  | [Component](63586110-d60f-f5a1-2bce-c5138003cbad.htm) | The Component class represents a component. A component is a modelling tool that typically  assembles multiple parts to build some type of a structure, for example a hall macro or at a  smaller scale a reinforcement component (a macro). Also, a custom part is a component. |
|  | [ComponentInput](2e678a2a-118b-ca18-2776-91cd29d4540c.htm) | The ComponentInput class handles the input of component objects and positions. A component has  one component input.  The component input must include all the needed input objects and points in the correct order.  For example,  an input with a point and a part is different from an input of a part and a point.  The maximum number of different input items in the collection is 10\. |
|  | [ConicalSurface](782c39eb-4018-ceec-cbf2-c8502d926da0.htm) | The ConicalSurface class defines a conical surface contour. |
|  | [ConicalSurfaceNode](73922bd2-0f50-6751-da49-df7948f18e6a.htm) | The ConicalSurfaceNode class represents conical surface geometry tree node. |
|  | [Connection](41a1ee09-b531-3160-137a-37aefe3f6947.htm) | The Connection class represents a connection. A connection is something that connects two or  more parts together. |
|  | [ConnectiveGeometry](f376b309-e3fe-c8f6-d8cd-805695550b9d.htm) | A class for geometry formed of several geometry sections. Geometry is initialized with polygon  geometry  and then can be extended by calling one of AddLeg methods using BentPlateGeometrySolver class.  In the case of success, two polygon geometries will be connected by cylindrical surface geometry  possibly  with help of additional polygon geometries.  Resulted geometry, then, can be set to bent plate. |
|  | [ConnectiveGeometryException](bb701f1a-d0bc-4b22-23ab-8484219793af.htm) | The ConnectiveGeometryException class represents an error that occurred during the  ConnectiveGeometry creation or modification. |
|  | [Contour](903abf10-4c92-e708-533a-88c7cebfd501.htm) | The Contour class defines a possibly chamfered contour. Contours must not have loops. |
|  | [ContourPlate](ec399c5b-d8e9-a69a-57c8-d85f70ac3c51.htm) | The ContourPlate class represents a part made with a contour, such as, a concrete slab. |
|  | [ContourPoint](1f158311-3d42-5ee3-4074-7cb13d653826.htm) | The ContourPoint class defines a point with possible chamfering information,  used, for example, to define a contour plate. |
|  | [ControlArc](5b51428a-00f9-155b-333c-83bd261a0b88.htm) | The ControlArc class defines a user defined arc helping in modeling work. |
|  | [ControlCircle](9763b8ff-1f52-2d69-7549-a6d8733e945c.htm) | The ControlCircle class defines a user defined (not magnetic) circle helping in modeling work.  If there are duplicated input points or 3 input points are in a line, ControlCircle.Insert()  will return false.  ControlCircle.Select() will return the center point of the circle to Point1\. |
|  | [ControlLine](8f08f0af-9bc7-d718-4bba-cd6f23c4b0e1.htm) | The ControlLine class defines a user defined (possibly magnetic) line helping in modeling work. |
|  | [ControlPlane](561ea178-df9a-d196-a846-e3223a8b202f.htm) | The ControlPlane class defines a user defined (possibly magnetic) plane helping in modeling  work. |
|  | [ControlPoint](38b3f184-d532-5d3e-d59e-2d16a7e0f2d9.htm) | The ControlPoint class defines a user defined point helping in modeling work. |
|  | [ControlPolycurve](cd91f00f-1681-cfc5-3616-ff8e229a29bc.htm) | The ControlPolycurve class defines a user defined polycurve object which contains a chain of  line and arc geometries. |
|  | [CurvedRebarGroup](9875d65f-111f-f5bb-6ba0-e8cb263099ab.htm) | The CurvedRebarGroup class represents a group of reinforcing bars which have a curved shape. |
|  | [CustomPart](d49ee520-e614-1f88-32b0-3bd442cfc84c.htm) | The CustomPart class represents a custom part object in the Tekla Structures model.  A custom part is a modeling tool that typically assembles multiple parts to build some  type of a beam\-like structure, for example a tapered beam or a sandwich panel. |
|  | [CutPlane](9ffbb991-b111-ad28-f0c0-5b9484c1002a.htm) | The CutPlane class defines how the end of a part is cut with a plane. A cut plane differs from a  fitting because  a cut can never extend the boundaries of the original part. |
|  | [CylindricalSurface](79e12062-9cfd-f132-b719-45e61c809615.htm) | The CylindricalSurface class defines a cylindrical surface contour. |
|  | [CylindricalSurfaceNode](647c9194-6cfd-7361-719f-9107ecae25a6.htm) | The CylindricalSurfaceNode class represents cylindrical surface geometry tree node. |
|  | [DeformingData](d344d31d-6c1a-e537-ddf0-57d0a2c0a48f.htm) | The DeformingData class holds information about the deforming of parts.  Deformed parts are parts that have been warped, cambered or shortened. |
|  | [Detail](5e5bcfd3-7bef-21c3-0c09-059814ebdebb.htm) | The Detail class represents a detail. A detail is different from a connection since the detail  only connects to one part. |
|  | [DisposableToken](6fceaf49-8ef1-a334-d72d-a109a1a627d9.htm) | [IDisposable](https://learn.microsoft.com/dotnet/api/system.idisposable) delegate adapter. |
|  | [EdgeChamfer](803ad6ff-2940-2bff-01b5-0241125e38b5.htm) | The EdgeChamfer class defines how the part edge is chamfered. |
|  | [Events](8718989a-ebeb-cbd0-b920-08fb7a8ad3e4.htm) | The Events class allows the user to register event listeners for model events. |
|  | [ExtensionIntersectsWithPlateException](1e7f5097-9730-c720-48e0-e816e25bef98.htm) | The ExtensionIntersectsWithPlateException class represents an error when extension plate clashes  with plates. |
|  | [FacePerpendicularToIntersectionLineException](935fde75-f2c5-1d01-623f-d7a6b4c48c34.htm) | The FacePerpendicularToIntersectionLineException class represents an error when, face  perpendicular to intersection line. |
|  | [FacesAtAnObtuseAngleException](5a2bc09b-f29d-62ef-c502-50bfc1f8aa86.htm) | The FacesAtAnObtuseAngleException class represents an error when, faces to be connected are too  steep of an angle. |
|  | [FacesTooNearEachOtherException](3e31a78f-75c9-796d-7463-c0d60e28e905.htm) | The FacesTooNearEachOtherException class represents an error when, faces to be connected  overlap. |
|  | [Fitting](9bd2b3ed-c087-cb0c-f1ed-2c11a3e4c533.htm) | The Fitting class defines how the part end fits to a plane. A fitting can make the part either  longer or shorter. |
|  | [GeneralConnectiveGeometryException](9a296802-ce5e-ef31-9f8a-37c708592065.htm) | The GeneralConnectiveGeometryException class represents a general error that occurred during the  ConnectiveGeometry creation or modification. |
|  | [GeometrySection](ebc2368c-cb3d-5533-8e3e-af3d02c7466d.htm) | The GeometrySection class represents geometry node with its identifier. |
|  | [GeometrySectionEnumerator](fabaac2a-bb59-e3d1-b60d-38f638e7bf6e.htm) | The GeometrySectionEnumerator class is used to enumerate the geometry sections of a bent plate  geometry. |
|  | [Grid](82142833-2bb4-61e8-88d3-e8b43a38ade2.htm) | The Grid class defines a user defined (possibly magnetic) set of planes helping in modeling  work. A grid has grid plane  instances as children. |
|  | [GridBase](6cd5d756-5f8e-15d5-37b7-728c940c30ed.htm) | The GridBase class defines the base class for grids. |
|  | [GridCylindricalSurface](49862649-da7c-2c72-554e-78cc2a2d7f6b.htm) | The GridCylindricalSurface class defines a user defined (possibly magnetic) cylindrical surface  helping in  modeling work. A grid cylindrical surface must always belong to a parent grid instance. |
|  | [GridPlane](d46eb5c5-4e0e-d205-47a5-61dd7d1bb1f9.htm) | The GridPlane class defines a user defined (possibly magnetic) plane helping in modeling work. A  grid plane must  always belong to a father grid instance. |
|  | [GridSurface](99d2617a-fb93-5d6e-c62d-bc84e0ee76c7.htm) | The GridSurface class defines a user defined (possibly magnetic) surface helping in modeling  work. A grid surface must  always belong to a parent GridBase instance. |
|  | [HierarchicDefinition](3b2e2665-3864-af76-83c7-ac2221f81a59.htm) | The HierarchicDefinition class defines a hierarchy structure. This hierarchy structure can  be instantiated and extended by hierarchical objects. |
|  | [HierarchicObject](c62fa47a-7ee7-9f7c-7151-313d6b9aad25.htm) | The HierarchicObject class defines an object in a tree\-structured hierarchy. The hierarchy  structure is defined  by hierarchical definitions which the hierarchical objects instantiate. Hierarchical objects may  contain  other hierarchical objects, thus forming a sub\-hierarchy, or model objects. |
|  | [InputItem](cc7681b2-4148-059a-f0f0-641b7c2d2769.htm) | The InputItem class is used to store input objects and positions. |
|  | [InvalidCurveCombinationException](aee41b14-a9b8-3cd3-84ff-3b08d60f94e6.htm) | This class represent an exception thrown when the combination of base curves is not allowed in a  lofted plate  operation |
|  | [InvalidFacePointsException](aec29813-439a-ea77-34ae-d2c1c3db7ef7.htm) | The InvalidFacePointsException class represents an error when, cannot create geometry from  requested face points. |
|  | [InvalidRadiusException](9f0fd914-78f1-fb5d-af93-9a736d9462d4.htm) | The InvalidRadiusException class represents an error when, cannot connect parts with a  cylindrical section having the provided radius. |
|  | [Load](d4147471-17dc-0a4b-f579-3f9f50fa93aa.htm) | The Load class is an abstract base class for all loads. |
|  | [LoadArea](0c92809d-6aa4-549b-023e-7879db4d7d61.htm) | The LoadArea class defines a linearly\-distributed force bound by a triangle or a quadrangle. |
|  | [LoadGroup](c33bc83e-1690-718a-c3e9-0a588cbd1943.htm) | The LoadGroup class implements grouping functionality related to all loads.  Each load should be assigned to a load group. Each load group contains loads  caused by the same action and to which you want to refer collectively.    Tekla Structures assumes that all loads in a group  - Have the same partial safety and other combination factors - Have the same action direction - Occur at the same time and all together      You may create new load groups, modify existing ones and delete  load groups via the .NET interface. You may also change the assigned load group  of a load and list all the load groups found in the model via the  ModelObjectSelector interface. The model always has at least one load group. |
|  | [LoadLine](6c2c4fcd-3944-0df3-0dfb-d042662860d1.htm) | The LoadLine class defines a linearly\-distributed force or torsion. |
|  | [LoadPoint](2d81d728-67f5-5d87-579e-5b33cdeb9b83.htm) | The LoadPoint class defines a concentrated force or a bending moment. |
|  | [LoadTemperature](65ff2768-3dca-366e-b304-deef114b05f8.htm) | The [LoadTemperature](65ff2768-3dca-366e-b304-deef114b05f8.htm) class defines a  temperature change in a part, or a temperature difference between two part surfaces. |
|  | [LoadUniform](f2fcb15d-f861-c351-a847-901b47057015.htm) | The LoadUniform class defines a uniformly\-distributed force bounded by a polygon. |
|  | [LoftedPlate](a0265b09-ae24-4aa3-6d43-d03a19f8f923.htm) | This class represents a lofted plate |
|  | [LoftedPlateOperationException](de853339-6173-37a9-4b73-fc8db446420f.htm) | This empty class serves as a base (marker class) for all the exception thrown in lofted plate  operations |
|  | [LogicalWeld](fc9878e2-e8b0-356f-5c7c-d06b71bd3057.htm) | The LogicalWeld class represents a group of welds in the model.  A logical weld contains a list of children welds.  The primary properties need to be the same in all the children welds. |
|  | [Material](b76cd4d2-f863-0e66-174a-99dda6afc8d6.htm) | The Material class represents a single material that parts can be made of. |
|  | [Model](01eab525-e3d6-22d8-b31a-e4c733e03d43.htm) | The Model class represents a single model open in Tekla Structures.  Before interaction with the model, the user will have to create one  instance of this class. |
|  | [ModelHandler](4a2739ce-3c44-53ae-9246-2d6ce85d750b.htm) | The ModelHandler class provides information about the currently open Tekla Structures  model. |
|  | [ModelInfo](cc2d593e-65f0-07c0-e4ab-17c60fe4f221.htm) | The ModelInfo class provides information about the currently open Tekla Structures  model. |
|  | [ModelObject](a90863bf-5ccc-e808-566a-a2ef79a9224d.htm) | The ModelObject class is an abstract base class for all model objects, such as parts, bolts,  welds and reinforcements. |
|  | [ModelObjectEnumerator](dfa49e10-8481-338b-9448-aa086d991eb4.htm) | The ModelObjectEnumerator class provides the means to iterate through model object instances in  the  current model. |
|  | [ModelObjectSelector](50af1768-22fb-080e-f3d1-08b0da8199da.htm) | The ModelObjectSelector class can be used to make different model object selections  from the current model. |
|  | [NullRulingException](6a6c5f35-ba15-bf0c-ebff-7e205ead76fd.htm) | This class represent an exception thrown when a ruling of the lofted plate (i.e. the lines that  swipe the plate  surface between the base curves) would become zero because of a lofted plate operation |
|  | [NumberingSeries](8788e92a-0d78-4c24-a3cc-039b96c08789.htm) | The NumberingSeries class describes how an object is to be numbered. |
|  | [NumberingSeriesNullable](e2273fc8-03bf-259b-a74a-ae85efeca9e6.htm) | The NumberingSeriesNullable class describes how an object is to be numbered. |
|  | [Object](9e5dc86b-68fe-395d-5ad0-5d4ca084ab36.htm) | The Object class is an abstract base class for all the objects Tekla Structures has. |
|  | [Offset](288e8450-b840-d318-343e-9098448754b4.htm) | The Offset class defines the offset value of start points and end points. The offset is the  distance from the current work plane in the three global directions. |
|  | [Part](ac720ea3-a9ae-235b-d627-c9c37585b6ec.htm) | The Part class represents a part in the model.  A part can be either a beam, a polybeam or a contour plate. |
|  | [Phase](2d4746c9-dc38-07d8-c644-b450af02d77d.htm) | The Phase class defines a model object phase. |
|  | [PhaseCollection](8501ccf0-5464-8ee1-0155-52e30d1742a4.htm) | The PhaseCollection class handles the collection of the model phases. |
|  | [Plane](37ad1799-48c1-2b90-a52c-fd0e84b4ec46.htm) | The Plane class defines a plane in space using an origin, an X\-axis and a Y\-axis. |
|  | [PlateIntersectsWithIntersectionLineException](092874f5-d392-7d82-429f-f7a9167ca364.htm) | The PlateIntersectsWithIntersectionLineException class represents an error when, plate polygon  extends beyond intersection line. |
|  | [PointCloud](1b398fae-616f-2cfa-8940-23f4d30e11c5.htm) | Initializes a new instance of the [PointCloud](1b398fae-616f-2cfa-8940-23f4d30e11c5.htm) class. |
|  | [PolyBeam](d879e653-76ab-ce1d-7b09-7abcdd6fa22e.htm) | The PolyBeam class represents a continuous beam with a contour as input. |
|  | [Polygon](b08e87a3-a223-a38f-882e-91c412b7db5e.htm) | The Polygon class represents a polygon object that has its corners at the  given points. |
|  | [PolygonNode](8b8b4b86-6354-8422-b25e-3cb648755976.htm) | The PolygonNode class represents flat geometry tree node. |
|  | [PolygonWeld](4b43dd4d-bd93-e2a8-7bf6-03cd05b834d6.htm) | The PolygonWeld class represents a polygon weld in the model.  A polygon weld has a main part and a secondary part. |
|  | [Polymesh](eef01483-89f4-d8bc-17e6-420d6156db89.htm) | The Polygon class represents a polygon object that has its corners at the  given points. |
|  | [PolymeshEnumerator](03636ab7-e0d2-62e7-0be0-0ec9962228c9.htm) | The PolymeshEnumerator class is used to enumerate the polymesh of a pour's merged faces. |
|  | [Position](4fd3fb0d-31ad-371e-d499-4b623d412b61.htm) | The Position class defines how a part is positioned relative to the input. |
|  | [PourBreak](d794b218-b226-027e-7d13-52c04efc8734.htm) | The PourBreak class represents a pour break in a model. |
|  | [PourObject](6cc031f5-71e3-2274-74ef-5b12f9954ff7.htm) | The PourObject class represents a pour object in the model. |
|  | [PourUnit](ce3eec91-2dd7-6b90-ecd5-97f5017102c8.htm) | The PourUnit class represents a pour unit in the model. |
|  | [Profile](ee78af8a-1ea0-65e3-6b75-57945a009dae.htm) | The Profile class defines the form of a cross section. |
|  | [ProjectInfo](e7a57d92-16ad-f456-ecda-fc014e592028.htm) | The ProjectInfo class provides project information about the currently open Tekla Structures  model. |
|  | [RadialGrid](3a0e7bec-0713-864c-4214-a7925c5df74e.htm) | The RadialGrid class defines a user defined (possibly magnetic) set;  radial grid has grid planes and cylindrical grid planes as children |
|  | [RebarComplexGeometry](4fdf4193-1664-f040-0c9c-789b5e9443cf.htm) | The ReinforcingBar class represents a single physical reinforcing bar. It contains the curves  and bendings that define the geometry of the bar. |
|  | [RebarCranking](87bcf96b-78c0-5086-7639-26f9e1fefe60.htm) | The RebarCranking class represents the cranking of reinforcing bars at a [RebarSplitter](e862d1ea-64b1-1fe4-26a2-a92aa34bbd83.htm). |
|  | [RebarCrankingNullable](103b736f-aa8a-4005-0b09-ea6808049d23.htm) | The RebarCrankingNullable class represents the cranking of reinforcing bars at a [RebarEndDetailModifier](a9416b22-067a-33ec-7328-88b946f665d2.htm). |
|  | [RebarEndDetailModifier](a9416b22-067a-33ec-7328-88b946f665d2.htm) | The RebarEndDetailModifier class represents a modifier that can modify the characteristics of [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) reinforcing bars that pass  through it.  It can modify reinforcing bar end properties and will therefore affect the end of the  reinforcing bars it is nearest to. |
|  | [RebarGeometry](fbcee9dc-d383-f540-0cf3-ec991d935127.htm) | The RebarGeometry class represents a single physical reinforcing bar \- the building block of  a mesh, a rebar group and even a single rebar.  It contains the physical reinforcing bar points in 3D space. |
|  | [RebarGroup](d55cb006-1a87-bda0-7cf6-0a879b3c6c6b.htm) | The RebarGroup class represents a group of reinforcing bars. |
|  | [RebarGuideline](39c4ee42-992a-871b-bed2-b3665b791270.htm) | Defines a rebar guideline that is used in a [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm).  A [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) has a minimum of one rebar  guideline, the primary guideline. |
|  | [RebarHookData](d0a79869-e12f-9686-d440-b2fe47008803.htm) | The RebarHookData class defines the hook at the end of a reinforcing bar.  Hooks are used for anchoring purposes. |
|  | [RebarHookDataNullable](e74062d0-32e0-6406-59ca-959ba934408d.htm) | The RebarHookDataNullable class defines the hook at the end of a reinforcing bar. Hooks are used  for anchoring purposes. |
|  | [RebarLapping](148c7454-629c-faca-e0c8-956fb85a4ad2.htm) | The RebarLapping class represents the lapping of reinforcing bars at a [RebarSplitter](e862d1ea-64b1-1fe4-26a2-a92aa34bbd83.htm). |
|  | [RebarLeg](6d6067fc-12b2-75b5-12b6-55671ccce55f.htm) | This represents a leg of a rebar and is used in the [RebarComplexGeometry](4fdf4193-1664-f040-0c9c-789b5e9443cf.htm) class. |
|  | [RebarLegFace](dbf1e225-bc2c-43a3-2487-427fa0d12224.htm) | Defines a rebar leg face that is used in a [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm).  Rebar leg faces control how the [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm)  generates the reinforcing bars. |
|  | [RebarLegSurfaceObject](091450f3-68ea-a337-38cd-1b32ff9c2a00.htm) | The RebarLegSurfaceObject class represents a polymesh surface for generating rebar legs in a [RebarSet](1dcd28d9-7862-66ee-4bc5-71d372457f2b.htm). |
|  | [RebarLengthAdjustmentDataNullable](f01e81f5-5d30-9ee4-1d10-be6f2ad7cafa.htm) | The RebarLengthAdjustmentDataNullable class defines the length adjustment at the end of a  reinforcing bar affected by a [RebarEndDetailModifier](a9416b22-067a-33ec-7328-88b946f665d2.htm).  If a length adjustment property is null then that property will not be applied to the [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) generated reinforcing bars. |
|  | [RebarMesh](a385b67a-fd0e-e6fb-d1ef-db2d770dfc8a.htm) | The RebarMesh class represents a reinforcement mesh. |
|  | [RebarProperties](131721c2-c623-c3df-1f06-ff6a0ba3302a.htm) | The RebarProperties class defines the default properties of the reinforcing bars in a [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm). |
|  | [RebarPropertiesNullable](c532391c-a2bf-3795-52e9-e6bbea31ad1c.htm) | The RebarPropertiesNullable class defines the properties of the reinforcing bars affected by a  [RebarPropertyModifier](fccc6e86-8989-4082-2190-75f4fd3b4552.htm). |
|  | [RebarPropertyModifier](fccc6e86-8989-4082-2190-75f4fd3b4552.htm) | The RebarPropertyModifier class represents a modifier that can modify the characteristics of [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) reinforcing bars that pass  through it. |
|  | [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) | The RebarSet class represents a set of reinforcing bars. |
|  | [RebarSetAddition](87273ccd-8487-e959-e60e-db165b5a6b8f.htm) | The RebarSetAddition class can be used to add [RebarLegFace](dbf1e225-bc2c-43a3-2487-427fa0d12224.htm) objects to an existing [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm). |
|  | [RebarSpacing](05404a92-6125-9e64-38ac-784900b5a5da.htm) | The RebarSpacing class defines spacing properties for a [RebarGuideline](39c4ee42-992a-871b-bed2-b3665b791270.htm). |
|  | [RebarSpacing   ExactSpacing](8313a0b4-447c-2512-0509-31708a10f051.htm) | This class defines objects used in the exact spacing type. |
|  | [RebarSpacingZone](cf189735-28cc-b497-1dac-feb92431104f.htm) | The RebarSpacingZone class defines the properties of a single spacing zone.  The spacing properties of number of spaces, spacing and length are proposed properties that the  spacing algorithm uses as input when calculating the  final reinforcing bars spacing.  Depending on the RebarSpacingZone properties and any other rebar spacing zones defined on the  associated [RebarGuideline](39c4ee42-992a-871b-bed2-b3665b791270.htm) the spacing  algorithm may  determine a different final reinforcing bars spacing from the original proposed properties.  However the RebarSpacingZone properties will always contain the  original proposed values. |
|  | [RebarSplice](7989d6f9-a7df-43e3-a504-cd4c0b361b02.htm) | The RebarSplice class represents a splice between two reinforcements. |
|  | [RebarSplitter](e862d1ea-64b1-1fe4-26a2-a92aa34bbd83.htm) | The RebarSplitter class represents a modifier that can split the [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) reinforcing bars that pass  through it. |
|  | [RebarStrand](8ce96935-0139-196c-6a95-ffa5c1d4ad89.htm) | The RebarStrand class represents prestressed strands for concrete parts. |
|  | [RebarThreadingDataNullable](57d87a1e-cd45-eccf-35f1-73a6e5fba633.htm) | The RebarThreadingDataNullable class defines the threading properties at the end of a  reinforcing bar affected by a [RebarEndDetailModifier](a9416b22-067a-33ec-7328-88b946f665d2.htm).  If a threading property is null then that property will not be applied to the [RebarSet](f17a0c5b-46ec-bb51-0f38-6971aef88a48.htm) generated reinforcing bars. |
|  | [ReferenceModel](a1ca3d98-d440-e04c-ed85-901efed0470c.htm) | The ReferenceModel class contains methods related to reference models.  A reference model is a reference of an external model. |
|  | [ReferenceModelObject](98ca59de-9a53-e939-e397-12158eb2f840.htm) | The ReferenceModelObject class contains methods related to reference model objects.  A reference model object is a subobject of a reference model. |
|  | [Reinforcement](c3d81ba0-8bd9-6e21-d36d-e650c6a0ef17.htm) | The Reinforcement class represents a reinforcement in the model. A reinforcement can either be a  mesh,  a single rebar, a rebar group or a strand. |
|  | [Seam](99d98d23-1040-9c9e-cab2-4d89c1e43f1e.htm) | The Seam class represents a seam. A seam is something that connects a main part to other parts  along an edge. |
|  | [SelfIntersectingSurfaceException](9f7aca96-ef41-ae5f-d61a-43d8bc994304.htm) | This class represent an exception thrown when the an operation on a lofted plate has been  determined to cause  a self intersecting surface |
|  | [SingleRebar](f6ddf6c4-47c6-8017-1a14-7b6a9ddd4961.htm) | The SingleRebar class represents a single reinforcing bar. |
|  | [Solid](7d939b20-a22f-7370-299b-a5a9fee8e54e.htm) | The Solid class represents the physical object in the model created by a part instance.  A solid instance can be used to query the actual geometry of the part and intersect that  geometry with, for example, lines and planes. |
|  | [SpiralBeam](2b829f38-d9b1-d5ea-f9b5-68801bbfdcd3.htm) | A class for the spiral beam part. |
|  | [SpiralBeamDataException](031dfd58-7798-4ded-5a3a-3e35e02069d8.htm) | The SpiralBeamDataException class represents an error that occurred during the spiral beam  creation or modification. |
|  | [StrandUnbondingData](b532c1be-5eec-7820-26ff-12e6061d7c05.htm) | The StrandUnbondingData class represents the unbonding of a rebar strand. |
|  | [SurfaceObject](03dc457c-9884-1f10-6a99-390c401463b7.htm) | The SurfaceObject class represents a surface object in the model. Currently this class  only support dynamic surfaces whose geometries are determined by the parts or pours  they associate to. It is not allowed to modify the geometry of a dynamic surface on Open API.  The polymesh setter of this class throws . |
|  | [SurfaceTreatment](6726c2c8-455a-71c3-8c81-3443c27018f9.htm) | The SurfaceTreatment class defines a layer above a building element defining what a surface  looks like.  The surface could for example have a tiled look. |
|  | [Task](c36a21f1-71b0-e3ab-8db5-2f10414db8bb.htm) | The Task class defines a single building site task. It may contain parts, assemblies or other  tasks. Tasks may  have a hierarchy between them i.e. there are other tasks as subtasks for a parent task. Tasks  may also  depend on each other, have resources assigned to them or have a single worktype. |
|  | [TaskDependency](2a999834-8d4f-42de-83fc-d66316056fc2.htm) | The TaskDependency class represents a dependency between two task objects. Each task may depend  on many other tasks, but between two specific tasks only one type of a dependency may exist.    There are four types of dependencies:  - FINISH\_TO\_FINISH (FF) - FINISH\_TO\_START (FS) - START\_TO\_FINISH (SF) - START\_TO\_START (SS) |
|  | [TaskWorktype](97bac05f-2188-ce24-1011-6e2e97cc8e3a.htm) | The TaskWorktype class defines a single worktype for a task object. Each task may belong to only  one worktype. |
|  | [TransformationPlane](324b1565-2e6e-8847-6c8b-88ca12e2151d.htm) | The TransformationPlane class describes a transformation from global model coordinates  to local and back to global. |
|  | [UndefinedCurveDirectionException](b4d572bd-333a-26f2-458c-d688d2ca0c4e.htm) | The UndefinedCurveDirectionException class represents an error when, cannot make inward/outward  curve check. |
|  | [UnknownLoftedPlateErrorException](1b7dc228-870a-7be6-0bb6-cfc92a24ab32.htm) | This class represent an exception thrown when an operation on a lofted plate caused an error of  unknown origin |
|  | [UnsupportedChamferException](7ab3fa5a-0958-525d-91a2-87eaf92f798d.htm) | The UnsupportedChamferException class represents an error when, plates containing unsupported  chamfer information. |
|  | [Weld](0acd5a34-eab5-0e9a-4869-d7f825f3a608.htm) | The Weld class represents a normal weld in the model.  A normal weld has a main part and a secondary part. |
|  | [WorkPlaneHandler](ac187147-19d4-851c-7af5-19e217534818.htm) | The WorkPlaneHandler class contains methods for getting and setting  the current transformation plane. |



Structures



|  | Structure | Description |
| --- | --- | --- |
|  | [RebarSpacing   ExactSpacing   Element](6d0a7d41-926b-8adb-0ff7-ca117e9be98d.htm) | This structure is used to hold number and distance data. |
|  | [RebarSpacing   Offset](62642faf-3c5e-66fd-2e26-bd3811a02ee9.htm) | Defines parameters associated with the start and end of the spacing. |
|  | [ReferenceModel   Revision](2d3e9160-2d8e-2de7-7c4c-978d447e3d92.htm) | Reference model revision. |



Interfaces



|  | Interface | Description |
| --- | --- | --- |
|  | [IAssemblable](c937f46b-c437-8d96-0545-6067119dfea2.htm) | The IAssemblable interface dictates which model objects are capabable of belonging to an  assembly at the leaf level. |
|  | [IGeometryNode](d79a60dd-f84b-ce24-8bfa-a7a2f1cb3912.htm) | The IGeometryNode interface represents geometry tree node. This is implemented by concrete  classes for the various types of geometry nodes |
|  | [IGeometryNodeVisitor](526199de-8d7e-02d0-0e3a-2a1a0793cf8d.htm) | The IGeometryNodeVisitor interface is implemented by classes visiting geometry nodes |



Delegates



|  | Delegate | Description |
| --- | --- | --- |
|  | [Events   ClashCheckDoneDelegate](7beeecd1-ba63-d100-5429-958333a736e9.htm) | The delegate to use for clash check completion. |
|  | [Events   ClashDetectedDelegate](3a5c3f17-6601-d4e1-6e10-5358c1978eb6.htm) | The delegate to use for clash detection.  Encapsulates any method that takes a clash check data object as a parameter. |
|  | [Events   CommandStatusChangeDelegate](a18d14a2-bf19-91d7-d00f-e5815b76e55f.htm) | The delegate to use for command status change. |
|  | [Events   InterruptedDelegate](055e98a3-bab4-394b-2407-c89799aec5d4.htm) | The delegate to use for interrupted event |
|  | [Events   ModelChangedDelegate](da2bba46-3d2c-0843-4e56-750a766f331c.htm) | The delegate to use for database commit. |
|  | [Events   ModelLoadDelegate](5ff47b5e-6907-32b6-2927-2d88b765bb73.htm) | The delegate to use for model load. |
|  | [Events   ModelLoadInfoDelegate](aecd1bab-ce8a-ec50-1752-8338234d5baa.htm) | The delegate to use for extended model load. |
|  | [Events   ModelObjectChangedDelegate](0fb5c5db-fdf7-5bf8-6b41-dad52cb01933.htm) | The delegate to use for changed model objects.  ModelObject inside ChangeData contains only identifier information. If properties need to be  checked, Select() for object is required. |
|  | [Events   ModelObjectNumberedDelegate](845f67a0-ae66-a0e9-f511-a7bf3fd6898a.htm) | The delegate to use for model objects which are numbered.  ModelObjects contain only identifier information. If properties need to be checked, Select() for  object is required. |
|  | [Events   ModelSaveAsDelegate](1d7ece5c-9948-e002-d6f9-f171c73b88a1.htm) | The delegate to use for model save as. |
|  | [Events   ModelSaveDelegate](145a428e-581b-8c98-df8f-2bee359d9595.htm) | The delegate to use for model save. |
|  | [Events   ModelSaveInfoDelegate](bf917674-1611-c405-e798-55e4d1afa4e9.htm) | The delegate to use for model save with context information. |
|  | [Events   NumberingDelegate](e7ad68f1-6cba-7616-c9c7-ffe1140a0f13.htm) | The delegate to use for numbering. |
|  | [Events   ProjectInfoChangedDelegate](f7c4a1ff-5621-bb91-19d9-dc984645810f.htm) | The delegate to use for change in project info. |
|  | [Events   SelectionChangeDelegate](036c3eef-bcb7-3a75-86bf-3854c482d889.htm) | The delegate to use for selection change. |
|  | [Events   TeklaStructuresExitDelegate](6adc90d0-84db-6db6-d8d3-fffbd87aaca8.htm) | The delegate to use for Tekla Structures exit. |
|  | [Events   ViewCameraChangedDelegate](42ddeb84-7691-757c-8885-2d307dfa0933.htm) | The delegate to use for view camera changed event |



Enumerations



|  | Enumeration | Description |
| --- | --- | --- |
|  | [Assembly   AssemblyTypeEnum](b5783436-5017-c594-0f5f-3c437e0e1108.htm) | The assembly types. |
|  | [BasePoint   CoordinateSystemType](f91ad4ef-a27d-ecfe-2d60-5cc8fcdfbdd3.htm) | The type of the base points coordinate system. |
|  | [BaseRebarGroup   ExcludeTypeEnum](46465095-11b7-c672-27b6-5cf5578ea1fc.htm) | The different ways to exclude reinforcing bars from the group. |
|  | [BaseRebarGroup   RebarGroupSpacingTypeEnum](30e7f555-8816-41d5-f79f-e902c423bc81.htm) | The ways to distribute the reinforcing bars with different spacings. |
|  | [BaseRebarModifier   AffectedRebarEnum](240f68e0-8f7f-6483-bfc6-d46137879691.htm) | This enum allows the caller to specify which end of the bar is of interest when calling the  function GetAffectedBars. |
|  | [BaseRebarModifier   BarsAffectedEnum](68f81d64-7286-6118-c2e4-f659b15a0c06.htm) | The reinforcing bars affected. |
|  | [BaseWeld   WeldContourEnum](45f9adf5-15ab-ec1a-ee0f-d2630e1b191c.htm) | The weld contour. |
|  | [BaseWeld   WeldElectrodeClassificationEnum](30523b14-c433-6f00-03bb-ff542912152d.htm) | The weld electrode classification. |
|  | [BaseWeld   WeldFinishEnum](703b6027-cf2b-26da-c3b9-32edb1fba8ce.htm) | The weld finish. |
|  | [BaseWeld   WeldIntermittentTypeEnum](fb0677a7-651a-7a60-af8b-8c9be1e73b29.htm) | Weld intermittent types. |
|  | [BaseWeld   WeldNDTInspectionEnum](6d6eec0c-e0d5-cdca-9d63-08477735be8b.htm) | The weld NDT inspection level. |
|  | [BaseWeld   WeldPlacementTypeEnum](209c02ef-b1d1-5629-05ad-7f988523ce36.htm) | Weld placement types. |
|  | [BaseWeld   WeldPreparationTypeEnum](13526ea5-f367-ea94-529d-03e7bd7427ca.htm) | Weld preparation types. |
|  | [BaseWeld   WeldProcessTypeEnum](81695cfc-b575-4541-c469-e4e20507b795.htm) | The weld process type. |
|  | [BaseWeld   WeldTypeEnum](4371747e-9838-b687-e75b-06d27cbffb1e.htm) | The weld types. |
|  | [Beam   BeamTypeEnum](6151749e-0ba3-8d75-6127-b84f300dd30f.htm) | The beam types.  The strip and pad footings are valid only if the material type of the beam is concrete. |
|  | [BentPlate   BendShape](b5343f3c-931a-194b-ccc5-e1c29895b276.htm) | Enumerator to define different possibilities for bend shapes. |
|  | [BentPlateGeometrySolver   OperationStatus](6e3965fc-cced-c0c2-3025-63df350c92bd.htm) | Define possible statuses for geometry creation/modification commands. |
|  | [BoltGroup   BoltHoleTypeEnum](4875b00c-24a3-bd15-5b05-76b3c541f18c.htm) | The special hole type. |
|  | [BoltGroup   BoltPlainHoleTypeEnum](d1716b64-f135-3612-eaca-36a14f2341ec.htm) | The plain hole type. |
|  | [BoltGroup   BoltRotateSlotsEnum](b1a3f6e5-d6af-9968-310d-4de51286c668.htm) | The rotation of the slots (the holes). |
|  | [BoltGroup   BoltThreadInMaterialEnum](3db6886a-d653-ddc4-6543-8e645a77f6da.htm) | The thread in the material. |
|  | [BoltGroup   BoltTypeEnum](6983381d-847d-9348-a456-338ed39eeb56.htm) | The type of the bolt. |
|  | [BoltGroup   ErrorStatus](2c68335c-fae5-a806-5e6b-40bbb9a29738.htm) | Define possible statuses for geometry creation/modification commands. |
|  | [BooleanPart   BooleanTypeEnum](a103fb75-b005-bb97-51cc-c4f5ff5763af.htm) | Defines the boolean operation: an add or a cut. |
|  | [Chamfer   ChamferTypeEnum](e17f4130-3566-bee7-b126-0ddfa6a77eea.htm) | The basic shape type of the chamfer. |
|  | [ChangeData   ChangeSourceTypeEnum](fe62fb09-f708-2f31-f3d4-57c7300fe40e.htm) | The source types of changed event. |
|  | [ChangeData   ChangeTypeEnum](64a75766-987a-6ed2-0a2d-553e8507a5fc.htm) | The types of changed event. |
|  | [CircleRebarGroup   CircleRebarGroupStirrupTypeEnum](1053de24-3e25-9b11-8b1c-30adc1a537b7.htm) | The different stirrup types. |
|  | [ClashCheckData   ClashTypeEnum](ef3402da-08ed-9713-6f0e-fcd6e9bfe78f.htm) | An enumeration for the different clash types. |
|  | [ContourPlate   ContourPlateTypeEnum](22f8144f-78df-e35b-1d18-c9999523d61b.htm) | The contour plate types. |
|  | [ControlCircle   ControlCircleColorEnum](20466415-4abb-34c8-b445-f7a9e03810da.htm) | The different circle colors. |
|  | [ControlLine   ControlLineColorEnum](5be6efb4-cfe5-6f0b-1ebc-be8609d0bc05.htm) | The different line colors. |
|  | [ControlObjectColorEnum](de19d580-60b4-961b-dfb1-107560ed1ed2.htm) | The different colors used for control objects (ControlLine and ControlCircle have their own). |
|  | [ControlObjectLineType](1e738aca-83ee-237a-9285-eceb80bc6c51.htm) | The line types (the presentation of the line). |
|  | [EdgeChamfer   ChamferEndTypeEnum](bb703a65-2763-a1f7-5315-8973f2a01dd0.htm) | The end type of the edge chamfer. |
|  | [HierarchicDefinitionTypeEnum](07fc35c8-a364-8d68-e9cb-4798407bf2b7.htm) | Defines the different types of classification hierarchies. |
|  | [InputItem   InputTypeEnum](a0433c89-2537-7cbc-0224-d7f60ed163d3.htm) | Defines the type of the input. |
|  | [Load   LoadAttachmentEnum](a2ef5acf-8fd5-795e-e10a-3158afc3acfa.htm) | The load attachment. |
|  | [Load   LoadPartNamesEnum](1fac12d5-3ea1-bf0c-4173-ad9376ec2d9c.htm) | The load part names. |
|  | [Load   LoadSpanningEnum](2d4b6439-a7f7-2f14-8a1a-37e5ff6ca95a.htm) | The load spanning. |
|  | [LoadArea   AreaLoadFormEnum](38b0eec5-e459-c5fd-12d3-806d0256c95e.htm) | The area load form. |
|  | [LoadGroup   Colors](6f2a89bd-8ba4-973c-a2f5-f7cef79ba412.htm) | The possible display colors for loads in a load group. |
|  | [LoadGroup   LoadGroupDirection](b0c729c6-cfde-f097-72c0-1ca150c956e9.htm) | The possible directions. |
|  | [LoadGroup   LoadGroupType](5bf85407-b90c-398a-2192-3072566c32fd.htm) | The possible types for load groups. |
|  | [LoadLine   LineLoadFormEnum](73f495f9-6e26-28a8-1ef6-82e1c7b2b808.htm) | The line load form. |
|  | [LoftedPlate   LoftedPlateFaceTypeEnum](f535a70c-d17d-cb0d-60a6-f472d5ec5664.htm) | Lofted plate solid creation face types. |
|  | [ModelObject   ModelObjectEnum](40af6269-5d48-d7a0-3b34-95ef2f744c3e.htm) | All possible concrete model object subclasses are defined here. This enumeration can be used to  fetch certain types of objects from the Tekla Structures model. |
|  | [ModelObjectEnumerator   EnumeratorTypeEnum](d68984b3-09aa-57bf-5ecb-e89993e7a61c.htm) | The types of enumerator available. |
|  | [Part   CastUnitTypeEnum](d8d763ec-4bed-04c2-a930-17d0fb53de92.htm) | The cast unit types. |
|  | [PolyBeam   PolyBeamTypeEnum](252fe607-40e6-7326-862c-944f6c6e4513.htm) | The polybeam types. |
|  | [Polymesh   PolymeshCheckerFlags](9f06f9d1-a8fb-41f2-aa21-b962d632fcdb.htm) | Polymesh check flags, please refer to PolymeshHealthCheckEnum for the corresponding result  values. |
|  | [Polymesh   PolymeshHealthCheckEnum](d3116a3b-bd01-49c1-ee54-56b2e9a2fb30.htm) | Polymesh check error result codes. See the PolymeshCheckerFlags to see how to set the various  checks. |
|  | [Position   DepthEnum](c532ad57-9a3c-8754-bccc-797db0151372.htm) | The position in the depth sense. |
|  | [Position   PlaneEnum](c599df35-04b2-a919-1c2a-92c3b8be2a94.htm) | The position in the plane sense. |
|  | [Position   RotationEnum](fae3579c-28af-3001-0871-db7105a8daa3.htm) | The position in the rotational sense. |
|  | [RebarCranking   CrankedLengthTypeEnum](390ab6ef-4ab1-2619-5da5-a82f4bfba90f.htm) | The cranked length type. |
|  | [RebarCranking   CrankingTypeEnum](416eb182-2d11-0104-67c9-68a6a368a264.htm) | The cranking type. |
|  | [RebarCranking   CrankSideEnum](59095750-aed2-11db-e365-1bbd36c7edb6.htm) | The crank side. |
|  | [RebarCrankingNullable   EndCrankingTypeEnum](db0dacf9-363d-f0b3-37c1-4a9eb2eaba1c.htm) | The end cranking type. |
|  | [RebarEndDetailModifier   EndTypeEnum](7c2ac690-db81-fc87-b89b-d393d28171e8.htm) | The end type. |
|  | [RebarGroup   RebarGroupStirrupTypeEnum](74460d20-c421-c309-9d21-aa5fc3feb0a0.htm) | The different stirrup types. |
|  | [RebarHookData   RebarHookShapeEnum](b689fb8e-0a78-1764-54db-a24472dbe63e.htm) | The different hook shapes. |
|  | [RebarLapping   LappingTypeEnum](1ac21790-4121-b56e-1d33-6be04b81dfe7.htm) | The lapping type. |
|  | [RebarLapping   LapPlacementEnum](11808979-1497-c22c-6dba-ba217bd0bf64.htm) | The placement of the lap relative to the associated [RebarLegFace](dbf1e225-bc2c-43a3-2487-427fa0d12224.htm). |
|  | [RebarLapping   LapSideEnum](36e35f69-31fb-a0d7-8168-eeda986ce68d.htm) | The side of the split that the lap is located. |
|  | [RebarLeg   OriginEnum](3060efb6-4306-f18f-573a-867ae166bfd2.htm) | Enumerator for different leg origins. |
|  | [RebarLengthAdjustmentDataNullable   LengthAdjustmentTypeEnum](615c6899-28ab-0be7-6a9c-be73d79184eb.htm) | The length adjustment type. |
|  | [RebarMesh   RebarMeshCrossBarLocationEnum](4ae1fcc1-01e0-0245-8025-8cd06a8711c8.htm) | The ways to locate the crossing bars. |
|  | [RebarMesh   RebarMeshSpacingMethodEnum](202198a8-2a54-900b-26a8-3b25c55db19f.htm) | The ways to distribute the reinforcing bars with different spacings. |
|  | [RebarMesh   RebarMeshTypeEnum](a9f722d1-5248-ab18-8d02-39e78dee4e05.htm) | The different types of reinforcement meshes. |
|  | [RebarPropertyModifier   GroupingTypeEnum](c78cea4b-aa31-e9b6-1295-e07dfa3f8679.htm) | The grouping type. |
|  | [RebarSpacing   ExactSpacing   Validation](da987189-57da-6c11-3fdb-a97d436b256f.htm) | Defines values used in validation of exact spacing elements. |
|  | [RebarSpacing   ExcludeTypeEnum](74ba9b18-0f68-86c7-f4dd-9342a89de5aa.htm) | The different ways to exclude reinforcing bars from the spacing. |
|  | [RebarSpacing   OffsetEnum](4adf4df1-e121-c217-8ab3-e463d84f7be9.htm) | The offset distance type. |
|  | [RebarSpacing   SpacingType](9caee5b6-a3fd-09dd-da56-10a049e1f45a.htm) | Defines the different spacing types. |
|  | [RebarSpacingZone   LengthEnum](223a779e-0ae1-dcad-ff8c-52bcd3fe46f3.htm) | The length type. |
|  | [RebarSpacingZone   SpacingEnum](bb47f856-0f41-2b58-5a0c-0d59c8c0c37a.htm) | The spacing type. |
|  | [RebarSplice   RebarSpliceBarPositionsEnum](cdbe3eee-707a-0ae2-9131-b8237bc02d51.htm) | The bar group positions in the splice. |
|  | [RebarSplice   RebarSpliceTypeEnum](b63b4f78-1efe-c97c-e733-e7fee3435d99.htm) | The splice types. |
|  | [RebarSplitter   SplitTypeEnum](27e2d4a2-4414-58ac-6830-edf05f2ea5e7.htm) | The split type. |
|  | [RebarSplitter   StaggerTypeEnum](2c5b0cea-b4cf-ce97-321f-28514bca0952.htm) | The side of the split that the additional offset (stagger) is located. |
|  | [ReferenceModel   VisibilityEnum](2af7cd9d-3835-c661-a69c-a9f2cde183b7.htm) | The visibility type. |
|  | [Reinforcement   RebarGeometryOptionEnum](7108e0fe-54a6-1bb5-2c14-3a461eff6bda.htm) | Options for the function GetRebarGeometries. |
|  | [Reinforcement   RebarGeometrySimplificationTypeEnum](9138fa19-1a9b-02bc-4710-a8856a76edc3.htm) | The rebar geometry simplification type. |
|  | [Reinforcement   RebarOffsetTypeEnum](a0e850ad-1bda-6e5d-09b5-e64010191033.htm) | The different types of offsets. |
|  | [Solid   SolidCreationTypeEnum](91495004-3272-05f8-52b1-cdc3d386ea19.htm) | The creation type of the solid. |
|  | [SpiralBeam   ErrorStatus](96dd1b8d-e2ec-e21a-a908-854a9748bd21.htm) | Define possible statuses for geometry creation/modification commands. |
|  | [SurfaceTreatment   SurfaceColorEnum](220357a1-749a-c75a-62cc-651b54fe5e1f.htm) | The different surfacing colors. |
|  | [SurfaceTreatment   SurfaceTypeEnum](3f55bbef-2e2a-3aac-7081-a9e9fd68a52e.htm) | The different surfacing types. |
|  | [TaskDependency   DependencyTypeEnum](51995429-984b-e28d-1b25-adbb3a83fe37.htm) | The task dependency types. |
|  | [Weld   WeldPositionEnum](845f121d-e5ce-cfe1-1467-bd657060b631.htm) | The weld position. |






Copyright © 1992\-2023 Trimble Solutions Corporation and its licensors. All rights reserved.




