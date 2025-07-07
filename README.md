# GalleryLoader missnamed this is backend of the java legacy app.

# 📸 Studio Booking System — Multi-App Overview
github: gallery-loader java side left out the angular piece. to fix

This project consists of multiple AngularJS + Java web apps under development to build a full-featured Photo Studio Booking Platform.

The apps were designed to be modular, each handling a different part of the user experience (listing, booking, scheduling), simulating what it would be like as a team of integration sharing components in local development
3 Apps being considered for integration: 

App 1 Studio listings and call to action/ views of studios costs etc
App 2 Calendar Event  App - handles login calendar view passing a studio id in url saves to calendar rest of front end is NOT connected to back end. 
App 3 CalendarStudioApp -- the app that integrates it all. 

# 🔹 App 1: Studio Management App. 📸 Photo Studio Listing App — Project Overview

# 🧾 Purpose

Displays a list of available photo studios, their galleries, and booking options.


# 🧱 Stack
Frontend: AngularJS 1.x (UI-Router)

Backend: Spring + Hibernate (JSP-based views)

DB: MySQL (via MAMP)

# 📂 Features
Loads studio list on launch

Supports image galleries per studio (gallery and static_gallery)

Has AngularJS states defined for booking, cart, checkout, and calendar, but only some are implemented

Calendar and cart views are not fully functional — they belong to another app (see below)

# 🚧 Development Notes
Application auto-navigates to /listing via $state.go('listing')

States like /calendar, /pay, /cart are defined but do not have UI elements to trigger them

Some state views (calendar.jsp, checkout.html, etc.) are placeholders or part of other apps


# Version 1 

## ▶️ Default Landing State
Route: /listing

View: studiolist.jsp

Purpose: Displays a list of available photo studios
It provides information on the sales of rentals 

A listing of available and unavailable listings, 

Link to a studio gallery to 'Take a tour' -> navigates to booking /booking/:studioId

## 📅 Booking
Route: /booking/:studioId
View: studio-booking.jsp
Purpose: Landing Page of Studio  Information and link to view the studio. 



## 👁️ Studio Gallery
Route: /gallery/:studioId or /static_gallery/:studioId

View: studio-gallery.jsp or static_gallery.jsp

Purpose: Allows users to preview images for a specific studio




# 🛠️ Next Steps

Clean up unused or unrelated Angular states confuses people as this was a listing studio only portion. Attempt to integrate may have failed. just ignore as this is one component. Decouple or remove  components that are unused in this sample

Migrate to Angular CLI or modern frontend in future


