## Joana S. Tria
# Lab 6: Define Your REST API Endpoints

| Resource | HTTP Verb | Resource URL | Use Case |
| :---: | ----- | ----- | ----- |
| Animal | GET | /api/animals | Get all animals in the zoo |
|  | GET | /api/animals/{animal-id} | Get specific animal by ID |
|  | POST | /api/animals | Add a new animal to the zoo |
|  | PUT | /api/animals/{animal-id} | Update an animal's details |
|  | PATCH | /api/animals/{animal-id} | Update an animal's specific detail like if the animals hasEaten, isAsleep, isSick and the like |
|  | DELETE | /api/animals/{animal-id} | Remove an animal from the zoo |
|  | POST | /api/animals/{animal-id}/feed | Feed an animal |
|  | POST | /api/animals/{animal-id}/exercise | Exercise an animal |
|  | POST | /api/animals/{animal-id}/examine | Handler examines an animal |
|  | POST | /api/animals/{animal-id}/heal | Veterinarian heals an animal |
|  | POST | /api/animals/{animal-id}/sound | Used to trigger the makeSound method |
|  | POST | /api/animals/{animal-id}/roam | Used to trigger the roam method |
|  | GET | /api/animals/species/{species-id} | Get all animals by species |
| People | GET | /api/people | Get all people in the zoo (Manager, Veterinarian, Vendor, Handler, and Visitors) |
|  | GET | /api/people/{people-id} | Get a person's detail by ID |
|  | POST | /api/people | Register a new person (Veterinarian, Vendor, Handler, and Visitors) |
|  | POST | /api/people/{people-id}/goTo | Move person's location |
| Visitor | POST | /api/visitors/{visitor-id}/ticket | Visitor buys a ticket |
|  | POST | /api/visitors/{visitor-id}/enter | Visitor enters zoo after ticket is validated |
|  | POST | /api/visitors/{visitor-id}/enclosures/{enclosure-id} | Visitor visits a specific enclosure with optional RequestParam to feed animals |
|  | POST | /api/visitors/{visitor-id}/enclosures/{enclosure-id}/feed | Another way: more specific |
|  | POST | /api/visitors/{visitor-id}/shops/{shop-id} | Visitor visits a shop with optional RequestParam to make a purchase |
|  | POST | /api/visitors/{visitor-id}/shops/{shop-id}/purchase | Another way: more specific |
|  | POST | /api/visitors/{visitor-id}/hospital | Visitor visits the hospital with optional RequestParam to listen to a science lecture |
|  | POST | /api/visitors/{visitor-id}/hospital/listen | Another way: more specific |
|  | POST | /api/visitors/{visitor-id}/leave | Visitors leaves the zoo |
| Vendor | POST | /api/vendors/{vendor-id}/sell | Vendor sells an item |
| Handler | POST | /api/handlers/{handler-id}/feed/{animal-id} | Handler feeds assigned animals |
|  | POST | /api/handlers/{handler-id}/exercise/{animal-id} | Handler exercise assigned animals |
|  | POST | /api/handlers/{handler-id}/examine/{animal-id} | Handler examine assigned animals |
| Veterinarian | POST | /api/veterinarian/{veterinarian-id}/lecture | Veterinarian gives a Science lecture |
| Manager | POST | /api/manager/{manager-id}/open | Manager opens the zoo |
|  | POST | /api/manager/{manager-id}/open | Manager closes the zoo |
| Building | GET | /api/buildings | List all building in the zoo |
|  | GET | /api/buildings/{building-id} | Get a building's details |
| Enclosure | GET | /api/enclosures | View all enclosures in the zoo |
|  | GET | /api/enclosures/{enclosure-id} | Get details of a specific enclosure |
| Shop | GET | /api/shops | View all shops |
|  | GET | /api/shops/{shop-id} | Get details of a specific shop |
| Hospital | GET | /api/hospital | Get hospital information |
| Status | GET | /api/zoo/status | Get zoo status (open or close) |

