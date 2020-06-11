# ADA-Lab-3
ADA Laboratory Work Nr.3 st.gr. TI-191M Iuzvac Anatolie

## Event Sourcing

**Event sourcing** is a great way to atomically update state and publish events. The traditional way to persist an entity is to save its current state. Event sourcing uses a radically different, event-centric approach to persistence. A business object is persisted by storing a sequence of state changing events. Whenever an object’s state changes, a new event is appended to the sequence of events. Since that is one operation it is inherently atomic. A entity’s current state is reconstructed by replaying its events.

Event sourcing enables building a forward-compatible application architecture — the ability to add more applications in the future that need to process the same event but create a different materialized view.

## Event Sourcing Use Cases

### 1. Social Platform

Almost every modern Social Platform uses **Event Sourcing** for consistent updates user's views. Usage of **Event Sourcing** in Social Platforms is vital because considering amount of users that updates their profile resulting in updates almoste every millisecond requires solution to keep updated user's of latest user's posts.

### 2. Business Management Platform

Maintaining a Business using one of the available Business Management Platforms (one of which I worked on) is vital to keep the other co-workers which uses the same platform notified of all changes made by other co-workers, especially when the work is done on vital information for the business which consists in the information of the clients, therefore is reasonable to use **Event Sourcing** in order to update as soon as possible all the information changes made by other co-workers and to notify co-workers of changes.

### 3. eCommerce Platform

Developing an eCommerce Platform results in creation of big amount of components such as : Orders, Products, Carts, Payments etc. Would be wise to integrate **Event Sourcing** pattern in this kind of platforms to ease the communication between the components and to give the agility for the further development of other components that could interprate the same event otherwise than previous components. 
