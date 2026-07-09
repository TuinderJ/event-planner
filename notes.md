# Backend
---
## Data Structures
### Tables
#### Events
| Field | Value Type | Notes |
| --- | --- | --- |
| ID | id |  |
| name | string | The name of the event |
| date_time | date_time | This will be the date of the event and the time the event starts. |
| end_time | time (optional) | This will be when the event ends. It can be left blank |
| description | string | This will be a longer description of the event |
| owner | !TODO | How to id an owner |

#### Guests
| Field | Value Type | Notes |
| --- | --- | --- |
| event | event_id |  |
| name | string | This will be the full name that will be displayed |
| phone_number | phone_number |  |
| status | guest_status |  |
| adults_attending | u8 | Number of adults attending under this invitation |
| kids_attending | u8 | Number of children attending under this invitation |
| reason | string (optional) | This is where someone invited can choose to give a reason why they can't attend |

#### Menu
| Field | Value Type | Notes |
| --- | --- | --- |
| name | string |  |
| category | menu_category |  Main Meal, Side Dish, Desert, or Drink |
| type | menu_item_type | This is to denote if the menu item is a suggestion, required, or guest added |

### Enums
#### guest_status
- invited
- declined
- pending
- accepted

#### menu_category
- main_meal
- side_dish
- desert
- drink

#### menu_item_type
- suggestion
- required
- guest_added

### Custom Types
#### phone_number
10 digit number
