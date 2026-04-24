# AI for Everyone

**Course by:** Andrew Ng  
**Provider:** DeepLearning.AI  
**Source:** https://www.deeplearning.ai/courses/ai-for-everyone/

---

## Course Overview

AI is not only for engineers. This non-technical course helps you understand AI technologies and spot opportunities to apply AI to problems in your organization. You will see examples of what today's AI can – and cannot – do, and understand how AI is impacting society.

**Duration:** ~7 hours (4 weeks)  
**Level:** Beginner (No prior experience required)  
**Instructor:** Andrew Ng, Founder of DeepLearning.AI

---

## Table of Contents

- [Week 1: What is AI?](#week-1-what-is-ai)
- [Week 2: Building AI Projects](#week-2-building-ai-projects)
- [Week 3: Building AI in Your Company](#week-3-building-ai-in-your-company)
- [Week 4: AI and Society](#week-4-ai-and-society)

---

# WEEK 1: WHAT IS AI?

## Introduction

### AI Value Creation
- **AI is projected to create $13-22 trillion in value by 2033** (McKinsey Global Institute)

### AI Categories

**ANI (Artificial Narrow Intelligence)**
- Smart speaker, self-driving car, web search
- AI in farming and factories
- Focuses on doing one specific thing

**Generative AI (Generative Artificial Intelligence)**
- ChatGPT, Claude, Gemini, Midjourney
- Creates new high quality content such as text, images or audio
- More general purpose within its domain (Still ANI)

**AGI (Artificial General Intelligence)**
- Do anything a human can do
- Still theoretical/not yet achieved

---

## Machine Learning

### Definition
> "Field of study that gives computers the ability to learn without being explicitly programmed."  
> — Arthur Samuel (1959)

### Supervised Learning (Most Important AI Tool Today)

Supervised learning involves learning a mapping from **Input (A)** to **Output (B)**.

#### Common Applications

| Input (A) | Output (B) | Application |
|-----------|-----------|-------------|
| Email | Spam? (0/1) | Spam filtering |
| Audio | Text transcript | Speech recognition |
| English | Chinese | Machine translation |
| Ad, user info | Click? (0/1) | Online advertising |
| Image, radar info | Position of other cars | Self-driving car |
| Image of phone | Defect? (0/1) | Visual inspection |

### Why Now?

**Three key drivers:**
1. **Large neural networks** - More powerful models
2. **More data** - Exponential growth in available data
3. **Better computing** - GPUs and cloud computing

**Performance Relationship:**
- Performance improves with:
  - Larger neural networks
  - More data
- Traditional AI plateaus; neural networks keep improving with scale

---

## What is Data?

### Example Dataset: Housing Prices

| House (sq ft) | # Bedrooms | Price ($1000) |
|--------------|------------|---------------|
| 523 | 1 | 100 |
| 645 | 1 | 150 |
| 708 | 2 | 200 |
| 1034 | 3 | 300 |
| 2290 | 4 | 350 |
| 2545 | 4 | 440 |

### Acquiring Data

**Three main methods:**

1. **Manual labeling**
   - Example: Labeling images as "cat" or "not cat"
   - Human annotation of data

2. **Download from websites/partnerships**
   - Example: Machine fault detection data
   
   | Machine | Temperature (°C) | Pressure (psi) | Machine Fault |
   |---------|-----------------|----------------|---------------|
   | 17987 | 60 | 7.65 | N |
   | 34672 | 100 | 25.50 | N |
   | 08542 | 140 | 75.50 | Y |
   | 98536 | 165 | 125.00 | Y |

3. **From observing user behaviors**
   - Example: E-commerce purchase data
   
   | User ID | Time | Price ($) | Purchased |
   |---------|------|-----------|-----------|
   | 4783 | Jan 21 08:15.20 | 7.95 | yes |
   | 3893 | March 3 11:30.15 | 10.00 | yes |
   | 8384 | June 11 14:15.05 | 9.50 | no |
   | 0931 | Aug 2 20:30.55 | 12.90 | yes |

### Use and Mis-use of Data

**Critical Reminder:**
> **Don't throw data at an AI team and assume it will be valuable. Data is messy.**

**Common Data Problems:**
- **Garbage in, garbage out**
- Incorrect labels
- Missing values
- Multiple types of data (images, audio, text - unstructured vs. structured)

**Example of Messy Data:**

| House (sq ft) | # Bedrooms | Price ($1000) |
|--------------|------------|---------------|
| 523 | 1 | 100 |
| 645 | 1 | 0.001 ❌ |
| 708 | unknown ❌ | 200 |
| 1034 | 3 | unknown ❌ |
| unknown ❌ | 4 | 350 |
| 2545 | unknown ❌ | 440 |

---

## The Terminology of AI

### Machine Learning vs. Data Science

**Same Dataset, Different Goals:**

| Size (sq ft) | # Bedrooms | # Bathrooms | Newly Renovated | Price ($1000) |
|-------------|------------|-------------|-----------------|---------------|
| 523 | 1 | 2 | N | 100 |
| 645 | 1 | 3 | N | 150 |
| 708 | 2 | 1 | N | 200 |
| 1034 | 3 | 3 | Y | 300 |
| 2290 | 4 | 4 | N | 350 |
| 2545 | 4 | 5 | Y | 440 |

**Machine Learning:**
- **Goal:** Running AI system (e.g., website/mobile app)
- **Output:** Automated predictions
- Example: Predict house prices for new listings

**Data Science:**
- **Goal:** Science of extracting knowledge and insights from data
- **Output:** Insights and recommendations
- Examples:
  - "Homes with 3 bedrooms are more expensive than homes with 2 bedrooms of a similar size"
  - "Newly renovated homes have a 15% premium"

### Deep Learning

**Key Points:**
- Neural networks were originally inspired by the brain
- **BUT:** The details of how they work are almost completely unrelated to how biological brains work
- Uses multiple layers to process information
- Very effective for unstructured data (images, audio, text)

**Example: Simple Neural Network**
```
Input: newly renovated, size, # bedrooms, # bathrooms
       ↓
    [neuron] ← big mathematical equation
       ↓
Output: price
```

### AI Has Many Tools

Beyond Machine Learning and Data Science:
- Deep learning / neural networks
- Unsupervised learning
- Graphical models
- Planning
- Knowledge graphs
- And more...

---

## What Makes an AI Company?

### A Lesson from the Rise of the Internet

Not every company using the internet became an "Internet company." Similarly, not every company using AI becomes an "AI company."

### AI Transformation

**The 5-Step Playbook:**
1. Execute pilot projects to gain momentum
2. Build an in-house AI team
3. Provide broad AI training
4. Develop an AI strategy
5. Develop internal and external communication

### Characteristics of True AI Companies

- **Strategic data acquisition** - Systematically collecting valuable data
- **Unified data warehouse** - Breaking down data silos
- **Pervasive automation** - AI integrated throughout
- **New job roles** - ML Engineers, Data Scientists
- **Virtuous cycle** - Better product → More users → More data → Better product

---

## What Machine Learning Can and Cannot Do

### The 1-Second Rule

**Rule of Thumb:**
> Anything you can do with 1 second of thought, we can probably now or soon automate.

### Supervised Learning: What Works Today

**Example: Customer Service Email Classification**

Input: User email
```
"The toy arrived two days late, so I wasn't able to give it 
to my niece for her birthday. Can I return it?"
```

Output: Classification
- ✓ Refund request
- Support
- Shipping

**What Happens When You Try Complex Responses:**

If asked to generate 2-3 paragraph responses:
- System with 1000 examples might produce: "Thank yes now your…" ❌
- Needs much more data and sophistication

### What Makes an ML Problem Easier

**Two key factors:**
1. **Learning a "simple" concept**
2. **Lots of data available**

### Real-World Examples

#### Self-Driving Car

**Can Do:**
- Detect stop signs, hitchhikers, bikes, turn signals
- Requires: High-quality labeled data

**Cannot Do:**
- Complex judgment in ambiguous situations
- Understanding human gestures in traffic
- Predicting unusual behavior

#### X-ray Diagnosis

**Can Do:**
- Diagnose pneumonia from ~10,000 labeled images
- High accuracy with sufficient training data

**Cannot Do:**
- Diagnose pneumonia from 10 images of a medical textbook chapter
- Generalize from small, different datasets

### Strengths and Weaknesses of Machine Learning

**ML Tends to Work Well When:**
1. Learning a "simple" function
2. There is lots of data available

**ML Tends to Work Poorly When:**
1. Learning complex functions from small amounts of data
2. Asked to perform on new types of data different from what it learned from

---

## Non-technical Explanation of Deep Learning (Optional)

### Example 1: Demand Prediction

**Simple Neural Network:**
```
Price → [neuron] → Demand
```

**Complex Neural Network:**
```
Price ────────┐
              │
Shipping cost ├──→ [multiple neurons] ──→ Demand
              │
Marketing ────┤
              │
Material ─────┘
```

The neural network automatically discovers:
- Which inputs matter
- Intermediate concepts
- How to combine information

### Example 2: Face Recognition

**Process Flow:**
```
Raw pixel values (30x10 grid of numbers)
    ↓
Edge detection
    ↓
Face parts detection
    ↓
Identity recognition
```

**Example pixel values:**
```
30  32  22  12  10  10  12  33  35  30
12  11  12 234 170 176  13  15  12  12
234 222 220 230 200 222 230 234  56  78
...
```

Each layer learns increasingly complex features automatically.

---

# WEEK 2: BUILDING AI PROJECTS

## Workflow of a Machine Learning Project

### Example: Speech Recognition

**Examples:** Amazon Echo/Alexa, Google Home, Apple Siri, Baidu DuerOS

### The 3 Key Steps

**1. Collect Data**
- Gather audio clips of people saying various words
- Include target words ("Ok Google") and many others
- Can take weeks to months

**2. Train Model**
- Use ML algorithm to learn input-to-output mappings
- **Critical:** Often the first attempt doesn't work very well
- **Iterate many times until good enough**
- Timeline: Days to months

**3. Deploy Model**
- Put model into production
- Get data back from real users
- Maintain/update model based on feedback
- Timeline: Days to months

**This is an iterative process, not linear!**

### Application to Other Domains

**Self-Driving Car:**
- Input: Image
- Output: Position of other cars
- Same 3-step process applies

---

## Workflow of a Data Science Project

### Example: Optimizing a Sales Funnel

**Sales Funnel Flow:**
```
Visit website → Product page → Shopping cart → Checkout
```

### The 3 Key Steps

**1. Collect Data**

Sample data collected:

| User ID | Country | Time | Webpage |
|---------|---------|------|---------|
| 2009 | Spain | 08:34:30 Jan 5 | home.html |
| 2897 | USA | 13:20:22 May 18 | redmug.html |
| 4893 | Philippines | 22:45:16 Jun 11 | mug.html |

**2. Analyze Data**
- Explore datasets
- Look for patterns
- **Iterate many times to get good insights**

**3. Suggest Hypotheses/Actions**
- Based on data insights
- Deploy changes
- Re-analyze new data periodically

### Example: Manufacturing Line

**Process:**
```
Mix clay → Shape mug → Add glaze → Fire kiln → Final inspection
```

**Data Collected:**

**Clay Data:**
| Batch # | Supplier | Mixing Time (min) |
|---------|----------|-------------------|
| 001 | ClayCo | 35 |
| 034 | GooClay | 22 |
| 109 | BrownStuff | 28 |

**Mug Data:**
| Batch # | Country | Humidity | Temp in Kiln (F) | Duration (hours) |
|---------|---------|----------|------------------|------------------|
| 301 | Spain | 0.002% | 1410° | 22 |
| 302 | USA | 0.003% | 1520° | 24 |
| 303 | Malaysia | 0.002% | 1420° | 22 |

---

## Every Job Function Needs to Learn How to Use Data

### Sales

**Machine Learning Application:**
- Automated lead sorting

Input data:
| Name | Title | Company Size | Email |
|------|-------|--------------|-------|
| Taylor | CEO | 3050 | tay@a.. |
| Janet | Manager | 230 | jan@b.. |
| David | Intern | 30 | dave@c.. |

Output: Priority (high/medium/low)

**Data Science Application:**
- Optimize sales funnel
- Analyze conversion rates at each stage

### Manufacturing

**Machine Learning Application:**
- Automated visual inspection
- Classify products: ok / ok / defect

**Data Science Application:**
- Optimize manufacturing line
- Analyze which processes affect quality

### Recruiting

**Machine Learning Application:**
- Automated resume screening
- Screen resumes: Yes / No

**Data Science Application:**
- Optimize recruiting funnel
- Email outreach → Phone screen → Onsite interview → Offer

### Marketing

**Machine Learning Application:**
- Customized product recommendations
- "Recommended for you" suggestions

**Data Science Application:**
- A/B testing
- Test different marketing approaches

### Agriculture

**Machine Learning Application:**
- Precision weed killing
- Automated identification and removal

**Data Science Application:**
- Crop analytics
- Optimize planting, watering, harvesting

---

## How to Choose an AI Project (Part 1)

### Brainstorming Framework

**The Sweet Spot:**
```
What AI can do  +  Things valuable for your business  =  AI Project
```

**Key Players:**
- **AI experts:** Understand what AI can do
- **Domain experts:** Understand what's valuable for business

### Brainstorming Tips

**Think About Tasks, Not Jobs:**
- Don't: "Automate radiologists"
- Do: "Help radiologists read scans faster"
- Don't: "Replace call center"
- Do: "Optimize call routing"

**Key Questions:**
- What are the main drivers of business value?
- What are the main pain points in your business?
- Where do you have bottlenecks?

### You Can Make Progress Even Without Big Data

**Important Points:**
- Having more data almost never hurts
- Data makes some businesses (like web search) defensible
- **But with small datasets, you might still make progress**

Don't let lack of data stop you from starting!

---

## How to Choose an AI Project (Part 2)

### Due Diligence Framework

**Technical Diligence + Business Diligence**

### Technical Diligence

**Key Questions:**
- Can AI system meet desired performance?
- How much data is needed?
- What is the engineering timeline?
- What are the technical risks?

**Evaluation Criteria:**
- Is this technically feasible with current AI?
- Do we have (or can we get) the required data?
- What accuracy is realistic?

### Business Diligence

**Impact Areas:**

**Current Business:**
- Lower costs?
- Increase revenue?
- Improve customer satisfaction?

**New Business:**
- Launch new product?
- Enter new market?
- Create new business model?

**ROI Calculation:**
- What's the expected return?
- What's the timeline to value?
- What are the risks?

### Build vs. Buy

**Decision Factors:**

**ML Projects:**
- Can be in-house or outsourced
- Consider team capabilities
- Consider strategic importance

**DS Projects:**
- More commonly in-house
- Requires deep business knowledge
- Harder to outsource effectively

**Industry Standard Components:**
- Avoid building these yourself
- Use existing solutions (e.g., speech recognition APIs)
- Focus on your unique value-add

---

## Working with an AI Team

### Specify Your Acceptance Criteria

**Example: Defect Detection**
- **Goal:** Detect defects with 95% accuracy
- **Dataset:** Provide AI team a dataset on which to measure performance
- Be clear and specific about what "success" means

### How AI Teams Think About Data

**Two Critical Datasets:**

**1. Training Set**
- Used to train the model
- The model learns patterns from this data

**2. Test Set**
- Used to evaluate performance
- Model has never seen this data before
- Simulates real-world performance

**Example:**
```
Training Set:        Test Set:
- ok                 - ok
- ok                 - ok
- ok                 - defect
- ok                 - ok
- defect
- ok
```

### Pitfall: Expecting 100% Accuracy

**Why 100% is Unrealistic:**

**1. Limitations of ML**
- Technology has inherent limits
- Some patterns are too complex

**2. Insufficient Data**
- May not have enough examples
- Data may not cover all scenarios

**3. Mislabeled Data**
- Humans make mistakes when labeling
- Introduces noise into training

**4. Ambiguous Labels**
- Some cases are genuinely ambiguous
- Even experts disagree

**Best Practice:** Set realistic accuracy targets based on:
- Current baseline performance
- Human-level performance
- Business requirements

---

## Technical Tools for AI Teams (Optional)

### Machine Learning Frameworks

**Popular Open-Source Frameworks:**
- TensorFlow
- PyTorch
- Keras
- MXNet
- CNTK
- Caffe
- PaddlePaddle
- Scikit-learn
- R
- Weka

### Open Source Resources

**Code Repositories:**
- GitHub (code sharing and collaboration)

**Research Publications:**
- Arxiv (pre-print research papers)

### Computing Infrastructure

**CPU (Computer Processor - Central Processing Unit)**
- General-purpose computing
- Good for training smaller models

**GPU (Graphics Processing Unit)**
- Specialized for parallel processing
- Much faster for deep learning
- Essential for large-scale training

**Deployment Options:**
- **Cloud:** Flexible, scalable, pay-as-you-go
- **On-premises:** More control, higher upfront cost

---

# WEEK 3: BUILDING AI IN YOUR COMPANY

## Case Study: Smart Speaker

### Examples
- Amazon Echo / Alexa
- Google Home
- Apple Siri
- Baidu DuerOS

### Example 1: "Hey device, tell me a joke"

**AI Pipeline - 4 Steps:**

**1. Trigger word/wakeword detection**
- Input: Audio
- Output: "Hey device"? (0/1)
- Constantly listening for trigger phrase

**2. Speech recognition**
- Input: Audio
- Output: "tell me a joke" (text)
- Converts audio to text

**3. Intent recognition**
- Input: "tell me a joke"
- Output: joke / time / music / call / weather
- Understands user's intent

**4. Execute joke**
- Runs specialized program
- Delivers the joke

**Flow Diagram:**
```
Audio → Trigger word detection → Speech recognition → Intent recognition → Execution
```

### Example 2: "Hey device, set timer for 10 minutes"

**Modified Pipeline:**

**Steps 1-3:** Same as above
- Trigger word detection
- Speech recognition
- Intent recognition

**Step 4:** Enhanced execution
- **4a:** Extract duration
  - "Set timer for 10 minutes" → 10 minutes
  - "Let me know when 10 minutes is up" → 10 minutes
- **4b:** Start timer with extracted duration

### Other Smart Speaker Functions

**Common capabilities:**
- Play music
- Volume up/down
- Make phone calls
- Tell current time
- Units conversion
- Answer simple questions
- Set alarms/timers
- Control smart home devices

**Key Insight:** Each function may require specialized AI components, but they share common infrastructure (trigger, speech recognition, intent).

---

## Case Study: Self-Driving Car

### Input Sensors
- **Image** (cameras)
- **Radar** (radio detection)
- **Lidar** (light detection)
- **GPS** (location)
- **Maps** (navigation data)

### Core AI Components

**Perception Tasks:**
1. **Car detection**
   - Identify other vehicles
   - Track their positions

2. **Pedestrian detection**
   - Identify people
   - Predict movements

3. **Lane detection**
   - Identify lane markings
   - Stay in lane

4. **Traffic light detection**
   - Recognize signals
   - Obey traffic laws

5. **Obstacle detection**
   - Identify barriers
   - Avoid collisions

**Prediction:**
6. **Trajectory prediction**
   - Predict where other objects will move
   - Anticipate behavior

**Planning:**
7. **Motion planning**
   - Decide where to go
   - Plan safe path

### Output: Control Commands
- **Steer**
- **Accelerate**
- **Brake**

**Complete Flow:**
```
Sensors (Image/Radar/Lidar + GPS + Maps)
    ↓
Perception (Car/Pedestrian/Lane/Traffic Light/Obstacle Detection)
    ↓
Trajectory Prediction
    ↓
Motion Planning
    ↓
Control (Steer/Accelerate/Brake)
```

---

## Example Roles of an AI Team

### Software Engineer
**Responsibilities:**
- Write production code
- Ensure reliability and scalability
- Example tasks: Joke execution, self-driving reliability
- **Typical team size:** 5-50+ people for AI projects

### Machine Learning Engineer
**Responsibilities:**
- Build ML systems (A→B mappings)
- Train and deploy models
- Optimize model performance
- Bridge research and production

### Machine Learning Researcher
**Responsibilities:**
- Extend state-of-the-art in ML
- Publish papers
- Develop new techniques
- **Note:** Often not needed for standard applications

### Applied ML Scientist
**Responsibilities:**
- Adapt existing techniques to new problems
- Read academic literature
- Find ways to apply research to products
- More common than pure researchers

### Data Scientist
**Responsibilities:**
- Examine data and provide insights
- Run experiments
- Make presentations to team/executives
- Answer business questions with data

### Data Engineer
**Responsibilities:**
- Organize data infrastructure
- Make sure data is saved in easily accessible way
- Ensure data security
- Optimize cost-effectiveness
- **Critical but often overlooked role**

### AI Product Manager
**Responsibilities:**
- Help decide what to build
- Determine what's feasible and valuable
- Work with teams to ship products
- Bridge business and technical

### Understanding Data Scale

**Common Measurements:**
- 1 MB (megabyte)
- 1,000 MB = 1 GB (gigabyte)
- 1,000,000 MB = 1 TB (terabyte)
- 1,000,000,000 MB = 1 PB (petabyte)

### Getting Started with a Small Team

**Three Options:**

**Option 1:** Minimal team
- 1 Software Engineer
- 1 Machine Learning Engineer/Data Scientist

**Option 2:** Even smaller
- 1 Software Engineer
- (Outsource ML/DS work)

**Option 3:** Bootstrap
- Nobody but yourself
- Learn and build incrementally

---

## AI Transformation Playbook (Part I)

### The 5-Step Process

**Complete Playbook:** https://landing.ai/ai-transformation-playbook/

### Step 1: Execute Pilot Projects to Gain Momentum

**Key Principles:**
- **More important for initial project to succeed** rather than be most valuable
- Success builds credibility and momentum
- **Show traction within 6-12 months**
- Can be in-house or outsourced

**Strategy:**
- Start with manageable, high-probability-of-success projects
- Quick wins demonstrate value
- Build team confidence and skills

### Step 2: Build an In-House AI Team

**Organizational Structure:**

```
CEO
 ├── CTO/CIO/CDO (or new CAIO - Chief AI Officer)
     └── Centralized AI Team
         ├── Business Unit 1 (later)
         ├── Business Unit 2 (later)
         └── Business Unit 3 (later)
```

**Evolution:**
1. **Initially:** Centralized AI team
   - Builds expertise
   - Shares knowledge
   - Establishes best practices

2. **Later:** Distribute to business units
   - After central team is established
   - Spread AI capabilities across organization

**Benefits:**
- Attracts talent better with dedicated team
- Builds critical mass of AI expertise
- Creates center of excellence

### Step 3: Provide Broad AI Training

**Training Matrix:**

| Role | Duration | What They Should Learn |
|------|----------|------------------------|
| **Executives and senior business leaders** | 4-12 hours | • What AI can do for your enterprise<br>• AI strategy<br>• Resource allocation |
| **Leaders of divisions working on AI projects** | 12+ hours | • Set project direction (technical and business diligence)<br>• Resource allocation<br>• Monitor progress |
| **AI engineer trainees** | 100+ hours | • Build and ship AI software<br>• Gather data<br>• Execute on specific AI projects |

**Key Insight:**
> The smart CLO (Chief Learning Officer) knows they should **curate** rather than **create** content.

**Training Sources:**
- Online courses (like this one)
- Industry conferences
- Internal workshops
- External experts
- Hands-on projects

---

## AI Transformation Playbook (Part II)

### Step 4: Develop an AI Strategy

**Core Principles:**
- Leverage AI to create advantage **specific to your industry sector**
- Don't just copy what others are doing
- Build unique competitive moats

### The Virtuous Cycle of AI

**Flywheel Effect:**
```
Better Product
     ↓
More Users
     ↓
More Data
     ↓
Better Product (cycle repeats)
```

**Strategy Considerations:**

**Data Strategy:**
- **Strategic data acquisition**
  - What data do we need?
  - How can we collect it systematically?
  
- **Unified data warehouse**
  - Break down data silos
  - Make data accessible across organization
  - Enable cross-functional insights

**Platform Advantages:**
- **Create network effects**
  - More users = more value for each user
  
- **Winner-take-all dynamics**
  - In some industries, AI can be an accelerator
  - First mover advantages may be significant

### Step 5: Develop Internal and External Communications

**Communication Strategy:**

**Investor Relations:**
- Communicate AI strategy and progress
- Demonstrate competitive advantage
- Show ROI and potential

**Government Relations:**
- Navigate regulatory landscape
- Participate in policy discussions
- Ensure compliance

**Customer/User Education:**
- Explain AI features and benefits
- Build trust in AI systems
- Manage expectations

**Talent/Recruitment:**
- Attract top AI talent
- Build employer brand
- Communicate exciting opportunities

**Internal Communications:**
- Keep organization aligned
- Share successes and learnings
- Build AI literacy across teams

---

## AI Pitfalls to Avoid

### Common Mistakes and Better Approaches

**❌ Don't: Expect AI to solve everything**
- AI has limitations
- Not every problem is an AI problem

**✓ Do: Be realistic about AI capabilities**
- Understand what AI can and cannot do
- Consider limitations of technology, data, and engineering resources
- Set appropriate expectations

---

**❌ Don't: Hire 2-3 ML engineers and count solely on them to come up with use cases**
- Engineering talent alone won't identify best opportunities
- Lack business context

**✓ Do: Pair engineering talent with business talent**
- Work cross-functionally
- Combine technical and domain expertise
- Find feasible AND valuable projects

---

**❌ Don't: Expect the AI project to work the first time**
- AI development is iterative
- First attempts often fail

**✓ Do: Plan for AI development to be iterative**
- Multiple attempts needed to succeed
- Expect failures and learning
- Build in time for experimentation

---

**❌ Don't: Expect traditional planning processes to apply without changes**
- Waterfall doesn't work well for AI
- Too much uncertainty upfront

**✓ Do: Work with AI team to establish appropriate processes**
- Agile/iterative approaches
- Timeline estimates with ranges
- Define milestones and KPIs
- Regular check-ins and adjustments

---

**❌ Don't: Think you need superstar AI engineers before you can do anything**
- Waiting for "perfect" team delays progress
- Learning happens by doing

**✓ Do: Keep building the team, but get going with what you have**
- Start with available talent
- Learn and improve
- Upgrade skills over time
- Hire as you grow

---

## Taking Your First Step in AI

### Initial Steps You Can Take

**1. Education**
- **Get friends to learn about AI**
  - Take this course together
  - Form a reading group
  - Discuss applications to your business

**2. Ideation**
- **Start brainstorming projects**
  - No project is too small
  - Focus on problems you understand
  - Look for quick wins

**3. Team Building**
- **Hire a few ML/DS people to help**
  - Even 1-2 people can start
  - They can guide strategy
  - Build internal capabilities

**4. Leadership**
- **Hire or appoint an AI leader**
  - VP AI, CAIO, or similar role
  - Someone to champion AI transformation
  - Coordinate efforts across organization

**5. Executive Engagement**
- **Discuss with CEO/Board possibilities of AI Transformation**
  - Key question: *Will your company be much more valuable and/or more effective if it were good at AI?*
  - Present opportunities and investments needed
  - Get buy-in for transformation journey

---

## Survey of Major AI Application Areas (Optional)

### Computer Vision

**Image Classification / Object Recognition:**
- Identify what's in an image
- Example: "cat" recognition

**Face Recognition:**
- Identify specific individuals
- Example: "Register new" face, recognize returning faces

**Object Detection:**
- Find and locate objects in images
- Draw bounding boxes around objects

**Image Segmentation:**
- Identify which pixels belong to which objects
- Detailed pixel-level classification

**Tracking:**
- Follow objects across video frames
- Maintain identity over time

---

### Natural Language Processing (NLP)

**Text Classification:**
- Categorize text into groups
- Examples:
  - Email → Spam/Non-Spam
  - Product description → Product category
  - Customer review → Sentiment (positive/negative)

**Sentiment Recognition:**
- "The food was good" → Positive
- "Service was horrible" → Negative

**Information Retrieval:**
- Web search
- Document search
- Question answering

**Named Entity Recognition:**
- Extract specific information from text
- Example: "Queen Elizabeth II knighted Sir Paul McCartney for his services to music at the Buckingham Palace."
  - Person: Queen Elizabeth II, Sir Paul McCartney
  - Location: Buckingham Palace
  - Event: knighting

**Machine Translation:**
- "AI is the new electricity" → "AIは、新たな電気だ" (Japanese)
- Translate between languages

**Others:**
- Parsing (understanding sentence structure)
- Part-of-speech tagging
  - "The cat on the mat"
  - Determiner, Noun, Preposition, Determiner, Noun

---

### Speech

**Speech Recognition (Speech-to-Text):**
- Convert spoken words to text
- Example: "The quick brown fox jumps over the lazy dog."

**Trigger Word/Wakeword Detection:**
- Detect specific phrases
- Example: "Hey Siri", "Alexa", "Ok Google"

**Speaker ID:**
- Identify who is speaking
- Voice authentication

**Speech Synthesis (Text-to-Speech, TTS):**
- Convert text to spoken audio
- Natural-sounding voices

---

### Robotics

**Three Core Components:**

**1. Perception:**
- Figuring out what's in the world around you
- Understanding environment

**2. Motion Planning:**
- Finding a path for the robot to follow
- Avoiding obstacles

**3. Control:**
- Sending commands to the motors
- Executing planned movements
- Following path precisely

---

### General Machine Learning

**Two Main Data Types:**

**Unstructured Data:**
- Images
- Audio
- Text
- No predefined structure

**Structured Data:**
- Database tables
- Spreadsheets
- Rows and columns

**Example Structured Data:**

| House Size (sq ft) | # Bedrooms | Price ($1000) |
|-------------------|------------|---------------|
| 523 | 1 | 100 |
| 645 | 1 | 150 |
| 708 | 2 | 200 |

**Example Manufacturing Data:**

| Clay Batch # | Supplier | Mixing Time (min) |
|-------------|----------|-------------------|
| 001 | ClayCo | 35 |
| 034 | GooClay | 22 |
| 109 | BrownStuff | 28 |

---

## Survey of Major AI Techniques (Optional)

### Unsupervised Learning

**Definition:**
- Given data **without** any specific desired output labels
- Find something interesting about the data

**Clustering:**
- Group similar items together
- Example: Finding cats from unlabeled YouTube videos

**Other Applications:**
- Customer segmentation
- Anomaly detection
- Pattern discovery

---

### Transfer Learning

**Concept:** Learn from task A, use knowledge to help on task B

**Example:**

**Task A: Car Detection**
- 100,000 images
- Well-trained model

**Task B: Golf Cart Detection**
- Only 100 images
- Use knowledge from car detection
- Much faster learning with less data

**Benefits:**
- Leverage existing models
- Need less data for new tasks
- Faster training

---

### Reinforcement Learning

**Concept:**
- Use a "reward signal" to tell the AI when it is doing well or poorly
- AI automatically learns to maximize its rewards

**Inputs Used:**
- GPS location
- Accelerometers (movement)
- Compass (direction)
- Other sensors

**Applications:**
- Game playing (Chess, Go, video games)
- Robotics control
- Autonomous navigation
- Resource optimization

**How it Works:**
- AI tries different actions
- Gets positive rewards for good outcomes
- Gets negative rewards for bad outcomes
- Learns optimal strategy over time

---

### GANs (Generative Adversarial Networks)

**Capability:**
- Synthesize new images from scratch
- Generate realistic-looking photos of things that don't exist

**Applications:**
- Create photorealistic faces
- Generate art
- Image enhancement
- Data augmentation

**Example:** Generate photos of people who don't actually exist

---

### Knowledge Graphs

**Concept:**
- Structured information storage
- Relationships between entities

**Example: Person Entity**
```
Ada Lovelace
├── Born: Dec 10, 1815
├── Died: Nov 27, 1852
└── Bio: English mathematician and writer...
```

**Example: Business Entity**
```
Northern Rooster Hotel
├── Address: 45 Rooster St, LA
├── Phone: (650) 555-3992
├── Wifi: yes
└── Pool: no
```

**Applications:**
- Search engines
- Recommendation systems
- Question answering
- Knowledge management

---

# WEEK 4: AI AND SOCIETY

## A Realistic View of AI

### The Goldilocks Rule for AI

**Three Perspectives:**

**❌ Too Optimistic:**
- Sentient / super-intelligent AI coming soon
- Killer robots will take over
- AGI is just around the corner

**❌ Too Pessimistic:**
- AI cannot do everything, so AI winter is coming
- No practical value
- All hype, no substance

**✓ Just Right:**
- AI can't do everything
- BUT will transform industries
- Significant practical value today
- Realistic about limitations and potential

---

## Limitations of AI

### Performance Limitations

**AI Has Bounds:**
- Cannot achieve perfect accuracy
- Struggles with certain types of problems
- Performance depends heavily on data quality and quantity

### Explainability is Hard

**The Black Box Problem:**
- Deep learning models are complex
- Difficult to explain why a decision was made
- **Sometimes doable** but requires special techniques

**Example: Medical Diagnosis**
- AI can detect right-sided pneumothorax (collapsed lung) in chest X-rays
- Can highlight relevant areas
- But explaining the exact reasoning is challenging

**Visualization Techniques:**
- Heat maps showing which parts of image influenced decision
- Saliency maps highlighting important features

### Biased AI Through Biased Data

**AI learns patterns from data, including biases**

### Adversarial Attacks on AI

**AI systems can be fooled with carefully crafted inputs**

---

## Discrimination / Bias

### AI Learning Unhealthy Stereotypes

**Word Embeddings Example:**

Mathematical relationships learned by AI:

**Appropriate relationships:**
- ✓ Man : Woman :: Father : Mother
- ✓ Man : Woman :: King : Queen

**Problematic relationship:**
- ✗ Man : Woman :: Computer Programmer : Homemaker

**Visual Representation:**
```
       Man (1,1) ────────── Computer Programmer (3,2)
          │                        │
          │                        │
       Woman (2,3) ───────────── Homemaker (4,4)
```

This reflects historical biases in training data, not reality.

### Why Bias Matters

**Real-World Harmful Examples:**

**1. Hiring Tool**
- Amazon's AI recruiting tool discriminated against women
- Trained on historical hiring data (mostly male hires)
- Learned to penalize resumes mentioning women's colleges or activities

**2. Facial Recognition**
- Systems matching dark-skinned individuals to criminal mugshots
- Higher error rates for women and people of color
- Trained primarily on light-skinned faces

**3. Bank Loan Approvals**
- Discriminatory lending decisions
- Perpetuating historical inequalities
- Denying opportunities based on biased patterns

**4. Reinforcing Stereotypes**
- Toxic effect of reinforcing unhealthy stereotypes
- Perpetuates harmful societal biases
- Can influence real-world decisions and opportunities

### Combating Bias

**Technical Solutions:**

1. **"Zero out" the bias in words**
   - Modify word embeddings to remove gender/race associations
   - Ensure equal representation in vector space

2. **Use less biased and/or more inclusive data**
   - Collect more diverse training data
   - Balance representation across demographics
   - Augment datasets to reduce imbalance

**Process Solutions:**

1. **Transparency and/or auditing processes**
   - Regular bias audits
   - Transparent methodology
   - Document limitations

2. **Diverse workforce**
   - Creates less biased applications
   - Multiple perspectives identify blind spots
   - Better understanding of impact on different groups

---

## Adversarial Attacks on AI

### Image Classification Attacks

**Small Perturbations Can Fool AI:**

**Example 1:**
- Original: Hummingbird (correctly classified)
- After minor perturbation: Hammer (incorrectly classified)
- **Human eyes see no difference**

**Example 2:**
- Original: Hare (correctly classified)
- After minor perturbation: Desk (incorrectly classified)
- Changes invisible to humans

### Physical Attacks

**Real-World Examples:**

**1. Stop Sign Attack**
- Special stickers placed on stop sign
- Self-driving car fails to see stop sign
- Dangerous safety implications

**2. Face Recognition Bypass**
- Specially designed glasses
- Can make person appear as someone else
- Example: Make AI think you're "Milla Jovovich"

**3. Adversarial Patch**
- Image of banana placed in scene
- AI misclassifies entire image
- Physical object can fool camera-based systems

### Adversarial Defenses

**Current State:**
- **Defenses do exist** but they incur some cost
- Trade-off between robustness and performance
- Ongoing research area

**Arms Race:**
- Similar to spam vs. anti-spam
- Or fraud vs. anti-fraud
- Attackers develop new techniques
- Defenders respond with countermeasures
- **Continuous evolution**

**Implications:**
- Critical for safety-critical applications
- Important for security systems
- Need ongoing vigilance

---

## Adverse Uses of AI

### Problematic Applications

**1. DeepFakes**
- Synthesize video of people doing things they never did
- Create fake videos of public figures
- Spread misinformation
- Damage reputations

**2. Undermining of Democracy and Privacy**
- Oppressive monitoring of individuals
- Mass surveillance
- Social control
- Authoritarian uses

**3. Generating Fake Comments**
- Astroturfing (fake grassroots movements)
- Manipulating public opinion
- Flooding comment sections
- Distorting democratic discourse

**4. Ongoing Arms Races**
- **Spam vs. anti-spam**
  - Spammers use AI to evade filters
  - Defenders use AI to detect spam
  
- **Fraud vs. anti-fraud**
  - Fraudsters use AI for attacks
  - Security teams use AI for detection

**Societal Challenge:**
- Need ethical guidelines
- Require regulation
- Importance of responsible AI development
- Balance innovation with safety

---

## AI and Developing Economies

### Opportunities to "Leapfrog"

**Historical Examples:**
- **Mobile phones**
  - Skipped landline infrastructure
  - Went directly to cellular
  
- **Mobile payments**
  - Many countries ahead of developed nations
  - M-Pesa in Kenya example
  
- **Online education**
  - Access to world-class education
  - Overcome infrastructure limitations

### How Developing Economies Can Build AI

**1. AI Communities are Still Immature Everywhere**
- **US and China are leading** but gaps are closeable
- Technology is still evolving rapidly
- Opportunities for innovation everywhere

**2. Focus on AI to Strengthen Country's Vertical Industries**
- Build on existing strengths
- Agriculture, manufacturing, services
- Solve local problems with AI

**3. Public-Private Partnerships**
- Government investment in infrastructure
- Private sector innovation
- Academic research collaboration
- Accelerate development

**Key Insight:**
- Don't just copy what US/China are doing
- Apply AI to unique local challenges
- Build competitive advantages in specific sectors

---

## AI and Jobs

### Impact on Employment

**Projected Changes by 2030:**

**Jobs Replaced:** 555-890 million  
**Jobs Created:** 400-800 million

*(Source: McKinsey Global Institute)*

**Key Insight:**
- Not just job destruction
- Also job creation
- Net effect varies by region and industry

### Automation Risk by Country

**Variation Across Countries:**
- Some countries more vulnerable than others
- Depends on:
  - Economic structure
  - Education levels
  - Industry composition
  - Ability to retrain workforce

**OECD Study Findings:**
- Significant variation in automation risk
- Jobs requiring creativity, social skills less at risk
- Routine cognitive and manual tasks more vulnerable

### Solutions

**1. Conditional Basic Income**
- Provide a safety net
- **BUT incentivize learning** and skill development
- Not universal basic income (UBI)
- Tied to education/training participation

**2. Lifelong Learning**
- Continuous education and retraining
- Adapt to changing job market
- Learn new skills throughout career
- Education system reform needed

**3. Political Solutions**
- Government policies to manage transition
- Investment in education and training
- Social safety nets
- Support for displaced workers

**Andrew Ng's Perspective:**
- Job displacement is real and deserves attention
- **NOT worried about:** Evil superintelligent AI (science fiction)
- **WORRIED about:** Near-term job displacement
- Focus on practical solutions

---
