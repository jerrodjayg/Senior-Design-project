# Senior-Design-project
# Confidential and Verifiable Audit Records for AI Workflows
# VCU CMSC 451 Senior Design Capstone Project
 
# PROJECT OVERVIEW
 
# This project is building a web application that lets organizations prove an AI system behaved correctly without exposing the sensitive data that the AI actually processed. Right now, when a company uses AI to make decisions (approving a loan, flagging a transaction, screening a resume, etc.), there is no easy way to later prove to an auditor, a regulator, or a customer that the AI followed the rules it was supposed to follow, because doing so usually means showing the original data, which is often private, confidential, or legally protected.
 
# Our system solves this by generating a cryptographically verifiable audit record every time the AI makes a decision. Instead of storing the raw data, the system creates a digital signature and a cryptographic commitment for each record, then organizes these commitments into a hash tree. This tree lets anyone later verify that a specific decision really happened, really came from the claimed AI process, and really followed the stated rules, all without seeing the underlying private data itself. Only the specific pieces of information someone is authorized to see are ever revealed, through a method called selective disclosure.
 
# In plain terms: the system creates a tamper-proof paper trail for AI decisions that can be checked and trusted by outside parties, while keeping the actual sensitive information locked away unless someone with the right permission specifically needs to see it.
 
# SPONSOR AND ADVISOR
 
# This project is sponsored by Virginia Commonwealth University (VCU) as part of the CMSC 451 Senior Design I and II sequence. Our faculty advisor is Dr. Hong-Sheng Zhou (hszhou@vcu.edu).
 
# TEAM
 
# Samuel Mushagasha - Project Manager. Oversees the project end to end, delegates work across the team, and assists in every area of the build (frontend, backend, database, and testing), with a primary focus on the database layer.
# Jerrod Jaygbay - Frontend Implementation Lead. Also responsible for logistics and financial tracking for the team.
# Samuel Brannen - Backend Implementation Lead. Also serves as the team's Systems/Manufacturing Engineer role for the course requirements.
# Kamarre Hicks - Test Engineer, responsible for leading quality assurance and verification efforts.
 
# All team members assist with testing across the application, regardless of their primary role.
 
# TECHNOLOGY STACK
 
# Frontend and Backend Framework: Next.js
# Database and Backend Services: Supabase
# Development Assistance: CodeEx AI Tool
# Core Logic and Cryptographic Processing: Python
 
# PROJECT PLAN
 
# The high-level plan is to:
 
# 1. Design the cryptographic architecture, including the signature scheme, the commitment scheme, and the hash tree structure used to batch and verify audit records.
# 2. Design the database schema in Supabase to store signed commitments, metadata, and access-control rules for selective disclosure.
# 3. Build the Next.js web application that lets users submit AI decision records, generate verifiable audit trails, and request selective disclosure of specific fields to authorized viewers.
# 4. Implement the Python-based cryptographic core that handles signing, committing, hashing, and verifying records, and connect it to the web application.
# 5. Test the full system end to end, including correctness of verification, performance of the hash tree under load, and security of the selective disclosure mechanism.
 
# All planning, diagrams, architecture design, and system design work is targeted for completion by November, so that implementation and coding can begin no later than December or January.
 
# BUDGET
 
# The only planned purchase for this project is a CodeX AI Tool membership at $20 per month, running from November through April.
 
# SOURCE CODE
 
# GitHub Repository: https://github.com/jerrodjayg/Senior-Design-project.git
 
# STATUS
 
# This project is currently in the planning and design phase. Architecture diagrams, concept evaluation, and the preliminary design proposal have been completed. Implementation is scheduled to begin in December or January, following VCU's CMSC 451/452 capstone timeline.