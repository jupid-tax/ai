# Technical Stack & Architecture

We're building AI-powered accounting for US businesses through native chat interfaces, with a technical stack designed for radical automation and new AI interaction paradigms.

## Core Infrastructure

  - Frontend: Next.js 15 (canary), React, TypeScript, Tailwind CSS
  - Backend: Supabase (auth/database), Vercel (primary), Google Cloud, Cloudflare, Turso
  - AI Services: 10+ providers (Anthropic, OpenAI, Google, Groq, xAI, DeepSeek, etc.)
  - Voice/Audio: ElevenLabs, Retell for AI voice conversations
  - Communications: Resend, native messaging APIs (iMessage, WhatsApp, Telegram)

## What Makes Our Approach Distinctive

  1. Native Chat as Primary Interface
  We don't build apps - we embed directly into iMessage, WhatsApp, and Telegram. Users interact with their AI accountant where they already communicate, eliminating app fatigue and meeting users in their
  existing workflows.

  2. Voice-First Accounting
  - AI robocalls for customer outreach and onboarding
  - Real-time audio conversations for complex accounting questions
  - Voice-based transaction categorization and expense tracking
  - Integration with ElevenLabs and Retell for natural conversations

  3. Extreme Automation Culture
  Our internal operations run on AI:
  - n8n workflows: AI classifies customer requests, routes to appropriate agents, triggers actions
  - Linear integration: AI agents create tasks, update priorities, assign team members
  - Analytics pipeline: PostHog events + Customer.io data → AI analysis → automated alerts
  - Session recordings: AI watches user sessions, identifies UX issues, creates improvement tasks
  - Every customer interaction generates data that feeds back into our AI systems

  4. Multi-Provider AI Orchestration
  - State machine architecture managing complex, multi-turn conversations
  - Automatic model routing (GPT-4 for analysis, Claude for writing, DeepSeek for reasoning)
  - Built-in reasoning trace extraction from models like DeepSeek R1
  - Stream-first design supporting real-time voice and text

  5. AI-Native Development Process
  We don't just build AI products - we build with AI:
  - IDE Stack: Claude Code, Cursor, Codex, OpenCode with custom enhancements
  - Task Master AI: Our meta-tool that manages development workflows
  - MCP Integrations: Browser automation, database access, API testing during development
  - Automated Testing: AI writes tests as we code, runs them continuously
  - Linear Automation: AI reviews PRs, updates task status, notifies stakeholders

  6. Self-Improving AI Systems
  Implementing DSPy-inspired architecture where:
  - Prompts evolve based on performance metrics, not manual tweaking
  - Each customer interaction improves the system
  - A/B testing happens automatically at the prompt level
  - Performance data from PostHog directly influences prompt evolution

  7. Financial AI Integration
  - Multi-provider banking (Plaid, Teller)
  - AI transaction categorization with continuous learning
  - Compliance automation through state machines
  - Real-time financial insights delivered via chat

## Technical Architecture for New Modalities

  Stream-First Everything: All interactions (text, voice, data) use streaming architecture, enabling real-time multi-modal experiences.

  Provider Abstraction Layer: Single interface supporting text, voice, vision, and reasoning models - add new modalities without changing application code.

  State Machine Core: Complex workflows (like LLC formation) managed through persistent state machines that work across chat, voice, and web interfaces.

  Native Integration Philosophy: We go where users are - messaging apps, voice calls, browser extensions - rather than forcing new interfaces.

## Why This Matters for New AI Interface Modalities

  We're not building another chatbot. We're proving that AI can integrate seamlessly into existing communication channels, handle voice as naturally as text, and improve itself without human intervention.
  Our technical stack isn't just ready for new modalities - it's actively exploring them in production with real customers handling real money.

  The combination of native chat interfaces, voice-first interactions, extreme automation, and self-improving AI systems positions us at the forefront of what AI interfaces will become: invisible,
  omnipresent, and continuously adapting to user needs.
