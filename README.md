# Design a complete PostgreSQL schema and secure functions for Momni, a care-sharing platform connecting families for childcare services with integrated social media features. The design should include:

DATABASE REQUIREMENTS:
1. Core Schema Requirements:
   - Implement role-based access control using a user_roles table with non-stacking roles
   - Define two special administrative roles: 
     * Financial Administrator: manages refunds, credits, and monetary operations
     * Community Administrator: handles user management, content moderation, and reporting
   - Support flexible family structures where:
     * Users can belong to multiple families
     * Users can create multiple families
     * Family creators have booking privileges for all family members
   - Enable hosting capabilities with:
     * Personal profiles
     * Family profiles
     * Host profiles with availability management
     * Host verification status tracking
   - Support Circle Up social media features through:
     * User-created circles with customizable privacy settings
     * Circle membership and moderation capabilities
     * Rich media content sharing within circles
     * Social interaction tracking (likes, comments, shares)

2. Safety and Verification Schema:
   - Background check tracking and renewal dates
   - Identity verification status and documents
   - Insurance documentation
   - Emergency contacts
   - Incident reporting
   - Review and rating system
   - Circle content moderation and reporting system
   - User behavior tracking and safety flags

3. Booking and Schedule Management:
   - Availability calendar with recurring slots
   - Booking status tracking
   - Waitlist management
   - Group booking capability
   - Cancellation policy enforcement
   - Special requirements tracking (allergies, medications, etc.)
   - Integration with circle events and activities

4. Financial Operations:
   - Payment processing and history
   - Refund tracking
   - Transaction dispute management
   - Tax document generation
   - Insurance verification
   - Circle-based group purchase capabilities
   - Event payment processing

5. Communication System:
   - Secure messaging between users
   - Notification preferences and history
   - Document sharing and storage
   - Emergency alert system
   - Circle-based group messaging
   - Content sharing permissions
   - Rich media support for circle communications

6. Circle Up Social Platform:
   - Circle management system:
     * Circle creation and configuration
     * Membership management
     * Privacy controls
     * Content moderation tools
   - Content management:
     * Multi-media post creation and storage
     * Content categorization and tagging
     * Content discovery and search
     * Trending content algorithms
   - Social interaction tracking:
     * User engagement metrics
     * Content performance analytics
     * Circle activity monitoring
     * Cross-circle interaction tracking

TECHNICAL REQUIREMENTS:
1. API Security:
   - All database operations must be performed through secure functions
   - API endpoints must be RESTful and JWT-authenticated
   - Implement row-level security where appropriate
   - Handle soft deletions for audit trails
   - Content access control based on circle privacy settings

2. Performance Considerations:
   - Include appropriate indexes
   - Implement efficient query patterns
   - Consider partitioning for large tables
   - Define appropriate cascade behaviors
   - Optimize for high-volume social interactions
   - Content delivery optimization
   - Real-time update handling

3. Documentation Requirements:
   - Full schema documentation with relationships
   - Function documentation with parameters and return values
   - API endpoint documentation
   - Security policy documentation
   - Example queries for common operations
   - Circle Up feature documentation
   - Content moderation guidelines
   - Privacy control documentation

Please provide:
1. Complete SQL schema with all tables, indexes, and constraints
2. Secure functions for all operations
3. API endpoint specifications
4. Security implementation details
5. Example queries for common operations
6. Performance optimization recommendations
7. Circle Up integration specifications
8. Content moderation workflows
9. Social feature scaling strategies
