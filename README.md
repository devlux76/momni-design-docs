Design a complete PostgreSQL schema and secure functions for Momni, a care-sharing platform connecting families for childcare services. The design should include:

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

2. Safety and Verification Schema:
   - Background check tracking and renewal dates
   - Identity verification status and documents
   - Insurance documentation
   - Emergency contacts
   - Incident reporting
   - Review and rating system

3. Booking and Schedule Management:
   - Availability calendar with recurring slots
   - Booking status tracking
   - Waitlist management
   - Group booking capability
   - Cancellation policy enforcement
   - Special requirements tracking (allergies, medications, etc.)

4. Financial Operations:
   - Payment processing and history
   - Refund tracking
   - Transaction dispute management
   - Tax document generation
   - Insurance verification

5. Communication System:
   - Secure messaging between users
   - Notification preferences and history
   - Document sharing and storage
   - Emergency alert system

TECHNICAL REQUIREMENTS:
1. API Security:
   - All database operations must be performed through secure functions
   - API endpoints must be RESTful and JWT-authenticated
   - Implement row-level security where appropriate
   - Handle soft deletions for audit trails

2. Performance Considerations:
   - Include appropriate indexes
   - Implement efficient query patterns
   - Consider partitioning for large tables
   - Define appropriate cascade behaviors

3. Documentation Requirements:
   - Full schema documentation with relationships
   - Function documentation with parameters and return values
   - API endpoint documentation
   - Security policy documentation
   - Example queries for common operations

Please provide:
1. Complete SQL schema with all tables, indexes, and constraints
2. Secure functions for all operations
3. API endpoint specifications
4. Security implementation details
5. Example queries for common operations
6. Performance optimization recommendations
