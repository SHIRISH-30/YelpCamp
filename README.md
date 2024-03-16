


# YelpCamp

YelpCamp is a Node.js web application project from the Udemy course - The Web Developer Bootcamp by Colt Steele. It is designed to allow users to add, rate, and review different campgrounds, enabling campers to share comments and concerns to help others plan their camping trips effectively.

## Features

- **Authentication:**
  - User login with username and password
- **Authorization:**
  - Users must be authenticated to manage posts and view user profiles
  - Users cannot edit or delete posts and comments created by other users
- **Manage campground posts with basic functionalities:**
  - Create, edit, and delete posts and comments
- **Upload campground photos**
- **Display campground location on MapBox**
- **Search existing campgrounds**
- **Manage user account with basic functionalities**
- **Flash messages responding to users' interactions with the app**
- **Responsive web design**
- **Update campground photos when editing campgrounds**

## API Reference

### List all campgrounds

```
GET /campgrounds
```

### Create a campground

```
POST /campgrounds/new
```

### Edit a campground

```
GET /campgrounds/:id/edit
```
**Parameters:**
- `id` (string, required): ID of the campground to edit
  - *Must be logged in and author to edit*

### Delete a campground

```
DELETE /campgrounds/:id
```
**Parameters:**
- `id` (string, required): ID of the campground to delete
  - *Must be logged in and author to delete*

### Add a review to a specific campground

```
POST /campgrounds/:id/reviews
```
**Parameters:**
- `id` (string, required): ID of the campground
  - *Must be logged in to review*

### Delete a review from a specific campground

```
DELETE /campgrounds/:id/reviews/:reviewId
```
**Parameters:**
- `id` (string, required): ID of the campground
- `reviewId` (string, required): ID of the review to delete
  - *Must be logged in and review owner to delete it*
```

Feel free to customize and expand this README as needed.
``` 

This README provides a clear structure outlining the features of the YelpCamp application along with its API endpoints and parameters. Adjustments can be made based on your preferences and requirements.
