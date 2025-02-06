# Momni Platform - Trust-Based Care-Sharing Network

## Overview
Momni is a platform enabling mothers to coordinate childcare within their trusted social circles, with optional expansion to public offerings. The core principle is that mothers are best positioned to make care decisions within their own social networks, while providing a pathway to offer care more broadly after verification.

## 1. Core Requirements

### 1.1 User Management
- Basic user profile:
  * Display name
  * Contact preferences
  * General location (city/neighborhood level only)
  * Profile photo (optional)
  * Brief bio
- Two administrative roles:
  * Financial Administrator: manages payments, refunds, credits
  * Community Administrator: handles content moderation, reporting

### 1.2 Circle Management (Primary Trust Network)
- Users can:
  * Create multiple circles
  * Join multiple circles
  * Set circle privacy levels
  * Manage circle membership
- Circle types:
  * Family circle (immediate family members)
  * Extended family circle
  * Friend circle
  * Neighborhood circle
  * Special interest circle (e.g., homeschool moms)
- Circle features:
  * Private messaging
  * Care availability sharing
  * Event planning
  * Resource sharing
  * Activity coordination

### 1.3 Care Coordination
- Within circles:
  * Share availability freely
  * Coordinate care swaps
  * Organize group activities
  * Track favors/exchanges
- Public listings (requires background_check=true):
  * Visible to users outside own circles
  * Enhanced profile visibility
  * Public availability calendar
  * Rate settings
  * Booking management

### 1.4 Social Features
- Content sharing:
  * Circle-specific posts
  * Event announcements
  * Activity planning
  * Resource recommendations
- Interaction tracking:
  * Comments
  * Reactions
  * RSVPs
  * Care coordination responses

## 2. Safety Features

### 2.1 Trust Network
- Circle-based trust system:
  * Care offerings visible only within joined circles by default
  * Circle creator approval for new members
  * Member removal capabilities
  * Circle privacy settings
- Public offering requirements:
  * Background check boolean flag
  * Enhanced profile requirements
  * Review system (public offerings only)

### 2.2 Safety Mechanisms
- Report system for inappropriate behavior
- Circle-level moderation tools
- Emergency contact system
- Incident reporting within circles
- Activity logging for safety

## 3. Booking and Scheduling

### 3.1 Circle-Based Coordination
- Availability sharing
- Care swap tracking
- Group activity planning
- Calendar integration
- Notification system

### 3.2 Public Booking (for verified hosts)
- Availability calendar
- Booking management
- Cancellation handling
- Payment processing
- Review system

## 4. Financial Operations

### 4.1 Circle-Based Exchange
- Care swap tracking
- Group expense sharing
- Activity cost splitting
- Payment handling for paid arrangements

### 4.2 Public Offering Payments
- Secure payment processing
- Refund management
- Transaction history
- Tax reporting support

## 5. Technical Requirements

### 5.1 Data Security
- Minimal PII collection
- End-to-end encryption for messages
- Circle content isolation
- Secure API endpoints
- Row-level security implementation

### 5.2 Performance Requirements
- Real-time messaging
- Calendar sync
- Notification delivery
- Content delivery optimization
- Mobile-first design support

### 5.3 Integration Points
- Background check status integration
- Payment processing
- Notification delivery
- Calendar systems
- Media storage

## 6. Implementation Deliverables

### 6.1 Database Schema
- Complete PostgreSQL schema
- Secure functions
- Access control policies
- Indexing strategy
- Partitioning plan

### 6.2 API Specification
- RESTful endpoint definitions
- Authentication requirements
- Rate limiting rules
- Response formats
- Error handling

### 6.3 Security Implementation
- Authentication system
- Authorization rules
- Data encryption
- Audit logging
- Privacy controls

### 6.4 Documentation
- Schema documentation
- API documentation
- Security documentation
- Integration guides
- Operational procedures

